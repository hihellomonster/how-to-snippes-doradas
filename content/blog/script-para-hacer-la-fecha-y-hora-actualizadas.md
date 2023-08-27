---
title: Conoer la fecha y hora actual 	
description: Así puedes obtener el DateTime con un simple script
date: 2023-08-27
draft: true
---
<style>
        .container {
            width: 100%;
            max-width: 900px;
            padding: 0 20px;
            margin: 0 auto;
            text-align: center;
            font-family: 'FiraCode Nerd Font Mono', 'FiraCode NF', 'Fira Code', 'Ubuntu Mono', 'Courier New', Courier, monospace;
        }
        
        .datetime {
            text-align: center;
        }
        
        #date {
            text-align: center;
        }
</style>

<div class="container">
    <p id="date">01/01/2020</p>
    <p id="time">00:00:00</p>
</div>

<script>
	var date = document.getElementById("date")
	var time = document.getElementById("time")

	var setTime = function() {
			date.innerHTML = new Date().toLocaleDateString("pt-br")
			time.innerHTML = new Date().toLocaleTimeString("pt-br")
	};

	setTime()

	setInterval(setTime, 1000)
</script>


### html

```html
<div class="container">
    <p id="date">01/01/2020</p>
    <p id="time">00:00:00</p>
</div>
```

### script

```js
var date = document.getElementById("date")
var time = document.getElementById("time")

var setTime = function() {
		date.innerHTML = new Date().toLocaleDateString("pt-br")
		time.innerHTML = new Date().toLocaleTimeString("pt-br")
};

setTime()

setInterval(setTime, 1000)
```
		
