# Unit 13: Geometric Optics

> Exam Weight: 12--15% | ~8--12 Class Periods

## Topics

### 13.1 Reflection
- The law of reflection states $\theta_i = \theta_r$: the outgoing ray makes the same angle with the normal as the incoming ray
- Both the incidence and reflection angles are referenced to the normal at the point of contact, not to the surface plane
- Specular reflection arises from smooth surfaces; because all normals point the same way, reflected rays remain parallel and a distinct image forms
- Diffuse reflection arises from rough surfaces; micro-scale variations in the normal direction scatter reflected rays broadly, preventing a coherent image
- A flat (plane) mirror creates a virtual, upright image that is the same size as the object
  - Image distance equals object distance: $d_i = d_o$
  - Magnification $m = +1$ (same size, upright)
  - The image exhibits lateral inversion (left and right are swapped)
  - The image appears to exist behind the mirror surface (virtual)

### 13.2 Images Formed by Mirrors
- Concave (converging) mirrors have an inward-curving reflecting surface with the center of curvature located on the same side as incoming light
  - Focal length is positive: $f > 0$
  - Incoming rays parallel to the axis meet at the focal point after reflection
  - Depending on how far the object is from the mirror, the resulting image can be real or virtual
- Convex (diverging) mirrors have an outward-curving reflecting surface with the center of curvature on the far (back) side
  - Focal length is negative: $f < 0$
  - Parallel rays spread apart after reflection; tracing them backward reveals a virtual focal point behind the mirror
  - These mirrors always produce a virtual, upright, and smaller-than-actual image
- Relationship between focal length and radius of curvature:

$$f = \frac{R}{2}$$

- Mirror equation:

$$\frac{1}{f} = \frac{1}{d_o} + \frac{1}{d_i}$$

- Magnification:

$$m = -\frac{d_i}{d_o} = \frac{h_i}{h_o}$$

- Sign conventions for mirrors:
  - $d_o > 0$: object sits in front of the mirror (real object)
  - $d_i > 0$: image forms in front of the mirror (real image)
  - $d_i < 0$: image forms behind the mirror (virtual image)
  - $m > 0$: image is upright; $m < 0$: image is inverted
  - $|m| > 1$: image is enlarged; $|m| < 1$: image is reduced
- Tracing three standard rays locates the image for a concave mirror:
  1. Parallel ray: travels in parallel to the axis, then reflects through the focal point
  2. Focal ray: passes through the focal point first, then reflects parallel to the axis
  3. Center ray: heads directly toward the center of curvature and reflects straight back along the same path

### 13.3 Refraction
- Refraction is the directional shift a light ray undergoes when it crosses from one transparent medium into another, caused by the change in propagation speed
- The refractive index is defined as $n = \frac{c}{v}$, where $c = 3.0 \times 10^8 \text{ m/s}$ is the speed of light in vacuum and $v$ is its speed in the medium
  - By definition $n \geq 1$; vacuum has $n = 1$ and air is approximately $n \approx 1.00$
  - A higher refractive index indicates that light moves more slowly through that material
- Snell's law:

$$n_1 \sin\theta_1 = n_2 \sin\theta_2$$

- Entering a medium with a higher refractive index: the ray bends toward the normal, so $\theta_2 < \theta_1$
- Entering a medium with a lower refractive index: the ray bends away from the normal, so $\theta_2 > \theta_1$
- Total internal reflection is triggered when light in a denser medium ($n_1 > n_2$) strikes the boundary at an incidence angle larger than the critical angle
- Critical angle:

$$\sin\theta_c = \frac{n_2}{n_1} \quad (n_1 > n_2)$$

- At the critical angle exactly, the refracted ray grazes the boundary at $\theta_2 = 90°$; for any larger angle, no refracted ray exists
- Real-world uses of total internal reflection include optical fiber data transmission and the reflecting prisms inside binoculars

### 13.4 Images Formed by Lenses
- A converging (convex) lens is thicker at its center than at its edges; it bends parallel rays so they meet at the focal point on the far side
  - Focal length is positive: $f > 0$
  - Image type (real or virtual) depends on where the object is placed relative to the focal point
- A diverging (concave) lens is thinner at its center; it spreads parallel rays apart so they appear to come from a virtual focal point on the same side as the incoming light
  - Focal length is negative: $f < 0$
  - This lens type always yields a virtual, upright, and diminished image regardless of object placement
- Thin lens equation:

$$\frac{1}{f} = \frac{1}{d_o} + \frac{1}{d_i}$$

- Magnification:

$$m = -\frac{d_i}{d_o} = \frac{h_i}{h_o}$$

- Sign conventions for lenses:
  - $d_o > 0$: object is on the side from which light arrives (real object)
  - $d_i > 0$: image forms on the opposite side of the lens from the object (real image)
  - $d_i < 0$: image forms on the same side of the lens as the object (virtual image)
  - $f > 0$: converging lens; $f < 0$: diverging lens
- Three standard rays used to construct a lens ray diagram:
  1. Parallel ray: enters parallel to the axis, then refracts through the far-side focal point
  2. Focal ray: passes through the near-side focal point first, then exits parallel to the axis
  3. Center ray: passes through the optical center of the lens with no deflection
- How image properties change with object position for a converging lens:
  - Object beyond $2f$: real, inverted, reduced
  - Object at $2f$: real, inverted, same size
  - Object between $f$ and $2f$: real, inverted, enlarged
  - Object at $f$: no image forms (refracted rays exit as a parallel beam)
  - Object inside $f$: virtual, upright, enlarged

## Skills to Master

- Use the law of reflection to predict where and how light bounces off a surface
- Contrast specular and diffuse reflection and account for the surface properties that produce each
- Solve for image position, size, and orientation using the mirror and magnification equations for curved mirrors
- Construct and read ray diagrams for plane mirrors, concave mirrors, and convex mirrors
- Calculate refraction angles at media boundaries by applying Snell's law
- Find the critical angle for a given pair of media and identify the conditions that trigger total internal reflection
- Determine image characteristics for converging and diverging lenses using the thin lens and magnification equations
- Construct and interpret ray diagrams for both lens types
- Correctly assign signs to object distance, image distance, and magnification to identify whether an image is real or virtual, upright or inverted, enlarged or reduced

## Core Concepts

1. In a uniform medium, light follows straight-line paths and can be analyzed using the ray model of geometric optics
2. Reflection obeys a simple symmetry rule: the incoming and outgoing rays make equal angles with the surface normal at the point of contact
3. Curved mirrors produce images whose distance, size, and orientation all follow from the mirror equation $\frac{1}{f} = \frac{1}{d_o} + \frac{1}{d_i}$ — the same relationship governs both concave and convex geometries
4. A change in wave speed at a boundary between two optical media causes light to change direction; the governing relation is Snell's law $n_1 \sin\theta_1 = n_2 \sin\theta_2$
5. The refractive index $n = c/v$ quantifies how much a medium slows light relative to vacuum; it is always $\geq 1$, and a higher value corresponds to a lower light speed
6. When light attempts to pass from an optically denser medium into a less dense one beyond the critical angle, the entire beam reflects back — no energy crosses the boundary
7. Thin lenses — whether converging or diverging — obey the same mathematical form as the mirror equation; the sign of $f$ distinguishes the two lens types
8. A real image forms at a point where light rays physically meet; a virtual image appears where backward extensions of the rays seem to originate, and cannot be captured on a screen

## Key Equations

### Reflection

$$\theta_i = \theta_r$$

### Mirror / Lens Equations

$$f = \frac{R}{2} \quad \text{(mirrors only)}$$

$$\frac{1}{f} = \frac{1}{d_o} + \frac{1}{d_i}$$

$$m = -\frac{d_i}{d_o} = \frac{h_i}{h_o}$$

### Refraction

$$n = \frac{c}{v}$$

$$n_1 \sin\theta_1 = n_2 \sin\theta_2$$

### Critical Angle (Total Internal Reflection)

$$\sin\theta_c = \frac{n_2}{n_1} \quad (n_1 > n_2)$$

## Key Terminology

| Term | Definition |
|------|-----------|
| **Normal** | A reference line drawn perpendicular to an optical surface at the exact point where a light ray strikes it |
| **Angle of incidence** | The angle formed between the incoming ray and the normal at the point of contact |
| **Angle of reflection** | The angle formed between the outgoing reflected ray and the normal at the point of contact |
| **Specular reflection** | Ordered reflection from a flat, polished surface where parallel incoming rays leave as parallel outgoing rays, producing a sharp image |
| **Diffuse reflection** | Disordered reflection from a rough surface where incoming parallel rays scatter in many different directions, producing no image |
| **Index of refraction ($n$)** | A dimensionless number equal to $c/v$, expressing how many times slower light travels in a medium compared to vacuum |
| **Refraction** | The change in direction of a light ray as it crosses the interface between two media with different refractive indices |
| **Total internal reflection** | A phenomenon in which all incident light is reflected back into the original medium because the angle of incidence exceeds the critical angle |
| **Critical angle ($\theta_c$)** | The smallest angle of incidence (measured from the normal) at which total internal reflection first occurs |
| **Real image** | An image formed at a location where light rays physically converge; it can be displayed on a screen |
| **Virtual image** | An image formed at a location from which light rays only appear to diverge; it cannot be displayed on a screen |
| **Focal point** | For a mirror or lens, the specific point at which incoming parallel rays converge — or from which they appear to diverge — after interacting with the optical element |
| **Focal length ($f$)** | The distance measured along the principal axis from the mirror or lens to its focal point |
| **Magnification ($m$)** | A signed ratio of image height to object height that simultaneously encodes image size ($|m|$) and orientation (sign of $m$) |
| **Principal axis** | The axis of symmetry of a mirror or lens — a straight line passing through the center of the optical surface at right angles to it |

## Common Misconceptions

1. **Angles of incidence and reflection are measured from the surface** -- Incorrect. Both angles are defined with respect to the normal — the line perpendicular to the surface at the point of contact — not from the surface itself.
2. **A virtual image is invisible because it is not "real"** -- Incorrect. The eye can detect virtual images perfectly well (your reflection in a bathroom mirror is a virtual image). The distinguishing feature is that virtual images cannot be focused onto a physical screen, because the light rays never actually meet at that location.
3. **Covering half of a lens or mirror removes half of the image** -- Incorrect. Each small region of the optical element collects rays from every point on the object and contributes to the full image. Blocking part of the surface dims the entire image by reducing the number of contributing rays, but the complete image persists.
4. **Light always changes direction when it enters a different medium** -- Not necessarily. A ray travelling exactly perpendicular to the boundary ($\theta_1 = 0°$) continues straight through without deflecting, even when the two media have very different refractive indices.
5. **A physically larger object will always produce a larger image** -- Incorrect. Image size is governed by the magnification equation $m = -d_i/d_o$, which depends entirely on where the object sits relative to the focal point — not on how large the object itself is.
6. **Total internal reflection can happen when light enters a denser medium** -- Incorrect. This phenomenon is restricted to light travelling from a higher-index medium into a lower-index one ($n_1 > n_2$). Light crossing into a denser medium always refracts rather than reflects completely.
7. **A mirror's focal length changes when it is submerged in water** -- Incorrect. Mirror focal length depends solely on the curvature of the reflecting surface via $f = R/2$ and is completely unaffected by the surrounding medium. Lenses, which work by refraction, do change their effective focal length with the surrounding medium.

## Units and Dimensional Analysis

| Quantity | SI Unit | Dimension |
|----------|---------|-----------|
| Angle of incidence / reflection / refraction | rad (radian) | dimensionless |
| Index of refraction ($n$) | (none) | dimensionless |
| Speed of light | m/s | [L][T]$^{-1}$ |
| Object distance ($d_o$) | m (meter) | [L] |
| Image distance ($d_i$) | m (meter) | [L] |
| Focal length ($f$) | m (meter) | [L] |
| Radius of curvature ($R$) | m (meter) | [L] |
| Object / image height ($h_o$, $h_i$) | m (meter) | [L] |
| Magnification ($m$) | (none) | dimensionless |
