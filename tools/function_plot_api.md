# function-plot.js API Reference & Style Guide

Use function-plot for mathematical function graphs: parabolas, sine waves, regression lines, error curves, distributions.

## Setup Pattern

```html
<div id="plot" style="width:800px;height:400px;margin:0 auto;"></div>
<script>
document.addEventListener('DOMContentLoaded', function() {
    if (typeof functionPlot === 'undefined') return;
    functionPlot({
        target: '#plot',
        width: 800,
        height: 400,
        xAxis: { domain: [0, 10], label: 'x' },
        yAxis: { domain: [0, 20], label: 'y' },
        data: [
            { fn: '-x^2 + 4*x + 5', color: '#e74c3c' }
        ]
    });
});
</script>
```

## ⚠️ MANDATORY Style Rules (for classroom readability)

### 1. Font Size — MUST override defaults (defaults are too small!)

After calling `functionPlot()`, apply these CSS overrides in a `<style>` block:

```css
/* Place this INSIDE the slide_html <style> or as inline <style> */
#plot .x.axis text, #plot .y.axis text {
    font-size: 16px !important;
    font-family: 'Segoe UI', Arial, sans-serif !important;
}
#plot .x.axis .label, #plot .y.axis .label {
    font-size: 18px !important;
    font-weight: 600 !important;
    font-family: 'Segoe UI', Arial, sans-serif !important;
}
```

### 2. Y-Axis Label — Do NOT use rotated text

function-plot rotates y-axis labels 90° by default — this is hard to read on projected slides. Instead:
- Use a **short** y-axis label (1-2 words max): `yAxis: { label: 'Height' }` not `yAxis: { label: 'Height of the ball in meters' }`
- Or **remove** the y-axis label and put it as a text annotation above the chart: `<div style="text-align:center;font-size:16px;margin-bottom:4px;">Height (meters) vs Time (seconds)</div>`

### 3. Domain — Set explicitly, don't rely on auto

Always set both `xAxis.domain` and `yAxis.domain` to ensure the important features (vertex, intercepts, key points) are visible:

```javascript
// BAD: auto domain might cut off the vertex
functionPlot({ target: '#plot', data: [{ fn: '-(x-2)^2+9' }] });

// GOOD: domain shows the full parabola including vertex
functionPlot({
    target: '#plot',
    width: 800, height: 400,
    xAxis: { domain: [-1, 5], label: 'x' },
    yAxis: { domain: [-2, 11], label: 'y' },
    data: [{ fn: '-(x-2)^2+9', color: '#e74c3c' }]
});
```

### 4. Colors — Use our standard palette

| Purpose | Color |
|---------|-------|
| Primary curve | `#e74c3c` (red) |
| Secondary curve | `#2196f3` (blue) |
| Tertiary curve | `#4caf50` (green) |
| Reference line | `#9e9e9e` (gray) |
| Highlight | `#ff9800` (orange) |

### 5. Grid — Enable for readability

```javascript
functionPlot({
    target: '#plot',
    grid: true,  // Shows grid lines
    // ...
});
```

## Annotations (key points, vertex, intercepts)

function-plot supports annotations for marking specific points:

```javascript
functionPlot({
    target: '#plot',
    width: 800, height: 400,
    xAxis: { domain: [-1, 5], label: 'Time (s)' },
    yAxis: { domain: [-2, 22], label: 'Height' },
    grid: true,
    data: [
        { fn: '-5*x^2 + 20*x', color: '#e74c3c', graphType: 'polyline' }
    ],
    annotations: [
        { x: 2, text: 'Vertex (2, 20)' },      // Vertical line at x=2
        { y: 20, text: 'Max height = 20m' }     // Horizontal line at y=20
    ]
});
```

## Multiple Functions

```javascript
data: [
    { fn: '-x^2 + 4*x + 5', color: '#e74c3c', graphType: 'polyline' },
    { fn: '2*x + 1', color: '#2196f3' },
    { fn: '0', color: '#9e9e9e', skipTip: true }  // x-axis reference
]
```

## Scatter Points (for worked examples)

```javascript
data: [
    { fn: '-5*x^2+20*x', color: '#e74c3c' },
    {
        points: [[0,0], [1,15], [2,20], [3,15], [4,0]],
        fnType: 'points',
        graphType: 'scatter',
        color: '#1565c0'
    }
]
```

## Complete Slide Example (classroom-ready)

```html
<div style="text-align:center;font-size:18px;font-weight:600;color:#37474f;margin-bottom:8px;">
    Basketball Height vs Time: h(t) = -5t² + 20t
</div>
<div id="physics-plot" style="width:800px;height:380px;margin:0 auto;"></div>
<style>
#physics-plot .x.axis text, #physics-plot .y.axis text { font-size: 16px !important; }
#physics-plot .x.axis .label, #physics-plot .y.axis .label { font-size: 18px !important; font-weight: 600 !important; }
</style>
<script>
document.addEventListener('DOMContentLoaded', function() {
    if (typeof functionPlot === 'undefined') return;
    functionPlot({
        target: '#physics-plot',
        width: 800, height: 380,
        grid: true,
        xAxis: { domain: [-0.5, 4.5], label: 'Time (seconds)' },
        yAxis: { domain: [-2, 22], label: 'Height (m)' },
        data: [
            { fn: '-5*x^2 + 20*x', color: '#e74c3c', graphType: 'polyline' },
            { points: [[2, 20]], fnType: 'points', graphType: 'scatter', color: '#1565c0' }
        ],
        annotations: [
            { x: 2, text: 'Peak at t = 2s' }
        ]
    });
});
</script>
```
