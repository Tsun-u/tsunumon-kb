# D3.js API Reference for Diagram Rendering (v7)

Use D3 for biology/natural science diagrams: cell cross-sections, vascular bundles, phylogenetic trees, organ schematics.

## Setup Pattern

```html
<svg id="diagram" width="500" height="400"></svg>
<script>
const svg = d3.select('#diagram');
// Build diagram with svg.append(...)
</script>
```

## Core Selection & Append

```javascript
const svg = d3.select('#id');          // Select element
svg.append('circle')                    // Append SVG element
   .attr('cx', 100).attr('cy', 100)    // Set attributes
   .attr('r', 50)
   .attr('fill', '#e53935')
   .attr('stroke', '#b71c1c')
   .attr('stroke-width', 1);

svg.append('line')
   .attr('x1', 0).attr('y1', 0)
   .attr('x2', 100).attr('y2', 100)
   .attr('stroke', '#333').attr('stroke-width', 2);

svg.append('rect')
   .attr('x', 10).attr('y', 10)
   .attr('width', 80).attr('height', 60)
   .attr('rx', 8)                       // Rounded corners
   .attr('fill', '#e3f2fd');

svg.append('text')
   .attr('x', 100).attr('y', 50)
   .attr('text-anchor', 'middle')       // center, start, end
   .attr('font-size', '16px')
   .attr('fill', '#333')
   .attr('stroke', '#fff')              // Text outline
   .attr('stroke-width', '3')
   .attr('paint-order', 'stroke fill')
   .text('Label');

svg.append('path')
   .attr('d', 'M10,80 Q50,10 90,80')   // Quadratic curve
   .attr('fill', 'none')
   .attr('stroke', '#2196f3');

svg.append('ellipse')
   .attr('cx', 150).attr('cy', 150)
   .attr('rx', 80).attr('ry', 50)
   .attr('fill', 'rgba(200,230,201,0.3)')
   .attr('stroke', '#2e7d32');
```

## Data-Driven Patterns (loops)

```javascript
// Ring arrangement (e.g., dicot vascular bundles)
const bundles = [];
for (let i = 0; i < 8; i++) {
    const angle = (i / 8) * Math.PI * 2;
    bundles.push({
        x: cx + Math.cos(angle) * radius,
        y: cy + Math.sin(angle) * radius
    });
}
svg.selectAll('.bundle')
   .data(bundles).enter()
   .append('circle')
   .attr('cx', d => d.x).attr('cy', d => d.y)
   .attr('r', 6).attr('fill', '#e53935');

// Scattered arrangement (e.g., monocot vascular bundles)
const scattered = [];
for (let i = 0; i < 20; i++) {
    let x, y, dist;
    do {
        x = cx + (Math.random() - 0.5) * range;
        y = cy + (Math.random() - 0.5) * range;
        dist = Math.sqrt((x - cx) ** 2 + (y - cy) ** 2);
    } while (dist > maxR || dist < minR);
    scattered.push({ x, y });
}

// Tree / branching (e.g., leaf veins, phylogenetic trees)
function drawBranch(svg, x1, y1, angle, length, depth) {
    if (depth === 0) return;
    const x2 = x1 + Math.cos(angle) * length;
    const y2 = y1 + Math.sin(angle) * length;
    svg.append('line')
       .attr('x1', x1).attr('y1', y1)
       .attr('x2', x2).attr('y2', y2)
       .attr('stroke', '#2e7d32')
       .attr('stroke-width', depth);
    drawBranch(svg, x2, y2, angle - 0.4, length * 0.7, depth - 1);
    drawBranch(svg, x2, y2, angle + 0.4, length * 0.7, depth - 1);
}
```

## Text Label Rules

All `<text>` elements MUST have:
- `font-size`: 14-24px
- `stroke` + `paint-order="stroke fill"` for outline
- `text-anchor` for alignment

```javascript
svg.append('text')
   .attr('font-size', '16px')
   .attr('stroke', '#fff')
   .attr('stroke-width', '3')
   .attr('paint-order', 'stroke fill')
   .attr('fill', '#333');
```
