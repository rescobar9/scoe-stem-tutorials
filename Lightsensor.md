# Lightsensor

## Step 1

Drag the ``||Basic:on start||`` block to the trash on the left main menu. 

In ``||Variables:Variables||``, make a variable and name it, ``||Variables:reading||``. 

## Step 2

In ``||Variables:Variables||``, drag the ``||Variables:set reading to 0||`` block inside the ``||Basic:forever||`` loop. 

```blocks
 basic.forever(function (){
reading = 0
})
```

## Step 3
Then from ``||Input:Input||``, drag the ``||Input:light level||`` block and replace the "0" in the ``||Variables:set reading to 0||``.

```blocks
 basic.forever(function (){
 let reading = input.lightLevel()
})
```

## Step 4
In ``||Basic:Basic||``, drag the ``||Basic:show number 0||`` block under the previous ``||Variables:set reading||`` ``||Input:light level||`` block.
```blocks
 basic.forever(function (){
 let reading = input.lightLevel()
basic.showNumber(0)
})
```
## Step 5
In``||Variables:Variables||``, drag the ``||Variables:reading||`` block and replace the "0" in the  ``||Basic:show number 0||`` block.
```blocks
 let reading = input.lightLevel()
basic.showNumber(reading)
})
```

## Step 6
In ``||Led:Led||``, drag the ``||Led:plot bar graph of 0 up to 0||`` block under the previous ``||Basic:show number 0||`` block.
```blocks
 basic.forever(function (){
 let reading = input.lightLevel()
basic.showNumber(reading)
led.plotBarGraph(0,0)
})
```

## Step 7
From ``||Variables:Variables||``", drag another ``||Variables:reading||`` block and replace the first 0 in the ``||Led:plot bar graph of 0 up to 0||`` block. Next, change the second 0 to 255.
```blocks
 basic.forever(function (){
 let reading = input.lightLevel()
basic.showNumber(reading)
led.plotBarGraph(reading,255)
})
```
## Step 8
Connect the Micro:bit to the USB port on your computer. Then click on "Download" (Make sure that you download the file to the Micro:bit drive")
```blocks
 basic.forever(function (){
 let reading = input.lightLevel()
basic.showNumber(reading)
led.plotBarGraph(reading,255)
})
```
## Step 9

Congratulations! You did it.

<script src="https://makecode.com/gh-pages-embed.js"></script><script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>
