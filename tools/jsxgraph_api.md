# JSXGraph API Reference (v1.11.1)

All elements are created via `board.create('elementType', params, attributes)`.

## Geometry Elements

| Element | Parameters | Description |
|---------|-----------|-------------|
| `point` | `[x, y]` | Free or fixed point |
| `midpoint` | `[p1, p2]` | Midpoint between two points |
| `line` | `[p1, p2]` | Infinite line through two points |
| `segment` | `[p1, p2]` | Line segment between two points |
| `polygon` | `[p1, p2, p3, ...]` | Closed polygon |
| `circle` | `[center, radius]` or `[center, point]` | Circle |
| `circumcircle` | `[p1, p2, p3]` | Circumscribed circle through three points |
| `circumcenter` | `[p1, p2, p3]` | Center of circumscribed circle |
| `incircle` | `[p1, p2, p3]` | Inscribed circle of triangle |
| `incenter` | `[p1, p2, p3]` | Center of inscribed circle |
| `arc` | `[center, p1, p2]` | Circular arc |
| `sector` | `[center, p1, p2]` | Circular sector |
| `angle` | `[p1, vertex, p2]` | Angle marker |
| `perpendicular` | `[line, point]` | Line perpendicular to `line` through `point` |
| `parallel` | `[line, point]` | Line parallel to `line` through `point` |
| `bisector` | `[p1, vertex, p2]` | Angle bisector |
| `tangent` | `[curve, point]` | Tangent line |
| `functiongraph` | `[function]` | Graph of y=f(x) |
| `curve` | `[xFunc, yFunc, tStart, tEnd]` | Parametric curve |
| `text` | `[x, y, 'content']` | Text label |
| `slider` | `[[x1,y1], [x2,y2], [min, val, max]]` | Interactive slider |
| `glider` | `[x, y, element]` | Point constrained to element |
| `reflection` | `[element, line]` | Reflection across line |

## ⚠️ DOES NOT EXIST — Common Mistakes

| ❌ Wrong | ✅ Correct way |
|----------|---------------|
| `perpendicularbisector` | Combine `midpoint` + `perpendicular` (see below) |
| `perpendicularBisector` | Same — does not exist |

## Perpendicular Bisector (correct pattern)

```javascript
// Perpendicular bisector of segment AB
var mid = board.create('midpoint', [A, B], { visible: false });
var line_AB = board.create('line', [A, B], { visible: false });
board.create('perpendicular', [line_AB, mid], {
    strokeColor: '#764ba2', strokeWidth: 1.5, dash: 2
});
```

## Common Attributes

```javascript
// Point
{ name: 'A', size: 5, color: '#1976d2',
  label: { fontSize: 18, fontWeight: 'bold',
    cssStyle: 'text-shadow: -1px -1px 0 #fff, 1px -1px 0 #fff, -1px 1px 0 #fff, 1px 1px 0 #fff' } }

// Circle / Circumcircle
{ strokeColor: '#e65100', strokeWidth: 2.5, dash: 2,
  fillColor: 'rgba(230,81,0,0.05)' }

// Line (visible: false for construction lines)
{ visible: false }

// Polygon
{ fillColor: 'rgba(255,193,7,0.1)', fillOpacity: 0.5,
  borders: { strokeColor: '#1976d2', strokeWidth: 2 } }
```

## Board Setup

```javascript
var board = JXG.JSXGraph.initBoard('container-id', {
    boundingbox: [-2, 10, 10, -2],  // [xmin, ymax, xmax, ymin]
    showNavigation: false,
    showCopyright: false,
    keepaspectratio: true  // ALWAYS use true for geometry
});
```

**IMPORTANT**: `boundingbox` must have enough padding so all elements (especially circumscribed circles) fit without clipping. Add at least 2 units beyond the extreme coordinates.

## Label Text Outline

JSXGraph labels are CSS-positioned `<div>` elements. Use `cssStyle` with `text-shadow` for outline:

```javascript
label: {
    fontSize: 18,
    fontWeight: 'bold',
    cssStyle: 'text-shadow: -1px -1px 0 #fff, 1px -1px 0 #fff, -1px 1px 0 #fff, 1px 1px 0 #fff'
}
```
