# Lightsensor

## Step 1

Make a variable and name it "reading" 

## Step 2

In "Variables", drag the "set reading to 0" block inside the forever loop. 

```blocks
 basic.forever(function (){
 var reading = 0
})
```

## Step 3
Then from "Input", drag the "light level" block and replace the "0".

```blocks
 basic.forever(function (){
 let reading = input.lightLevel()
})
```

## Step 4
From "Basic", drag the "show number 0" block under the previous block.
```blocks
 basic.forever(function (){
 let reading = input.lightLevel()
basic.showNumber(0)
})
```



<script src="https://makecode.com/gh-pages-embed.js"></script><script>makeCodeRender("{{ site.makecode.home_url }}", "{{ site.github.owner_name }}/{{ site.github.repository_name }}");</script>
