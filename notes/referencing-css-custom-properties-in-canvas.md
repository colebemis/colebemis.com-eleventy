---
title: Referencing CSS custom properties in canvas
date: 2020-12-25T00:26:17.282Z
---


```html
<style>
  :root {
    --my-color: #f00;
  }
</style>

<canvas id="my-canvas"></canvas>

<script>
  const canvasElement = document.getElementById('my-canvas')
  const ctx = canvasElement.getContext('2d')
  ctx.fillStyle = window.getComputedStyle(document.documentElement).getPropertyValue('--my-color')
  ctx.fillRect(10, 10, 150, 100)
</script>
```