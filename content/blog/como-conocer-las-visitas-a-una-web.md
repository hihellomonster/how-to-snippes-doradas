---
title: ¿Cuántas veces has visitado un sitio web?
description: Quieres conocer cuántas veces has visitado una página
date: 2023-08-26
tags:
  - localstorage
  - marketip
---
¿Quieres conocer el total de veces que has visitado una pagina? Con este script lo puedes conocer. Se utiliza un poco de localStorage. 
¿Para que la puedes utilizar el saber cuántas visitas tiene una página? para poder ofrecer algún premio, conocer la lealtad y/o interes en cierto sitio. 

# Code
```html
Gracias por tu visita número <span id="vecesVista"></span>
```
Gracias por tu visita número <span id="vecesVista"></span>

<script>
    if (!localStorage.pageLoadCount)
        localStorage.pageLoadCount = 0;
    localStorage.pageLoadCount = parseInt(localStorage.pageLoadCount) + 1;
    document.getElementById('vecesVista').textContent = localStorage.pageLoadCount;
</script>

```js
    if (!localStorage.pageLoadCount)
        localStorage.pageLoadCount = 0;
    localStorage.pageLoadCount = parseInt(localStorage.pageLoadCount) + 1;
    document.getElementById('vecesVista').textContent = localStorage.pageLoadCount;
```

