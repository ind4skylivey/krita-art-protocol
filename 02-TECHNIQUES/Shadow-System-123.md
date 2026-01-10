---
type: technique
artist: Mogoon
difficulty: ⭐⭐⭐⭐☆
tags: [core, shadows, anime, rendering]
---

# Shadow System 1-2-3

> [!quote] Philosophy
> Realism in anime doesn't come from the amount of detail, but from the correct hierarchy of light information.

This system divides shading into three distinct logical layers. It is the industry standard for semi-realistic styles (similar to WLOP/Mogoon).

## The Hierarchy

### 1️⃣ Shadow 1: The Form (Hard Edge)
Defines the basic geometry. It is binary: there is either light or no light.
- **Krita Tool:** `Basic-5 Size` (Hard edge) or `Ink-4 Pen Rough`.
- **Location:** Terminator line. Where light stops touching the surface.
- **Common Error:** Making it blurry. **KEEP IT HARD**.
- **Color:** Base tone shifted towards cool colors + higher saturation.

### 2️⃣ Shadow 2: The Transition (Soft Edge)
Softens the form and simulates "subsurface scattering" (light bouncing under the skin).
- **Krita Tool:** `Airbrush Soft` or `Blender Blur`.
- **Action:** Soften *only* the edge of Shadow 1 facing the light, or apply large gradients over Shadow 1.
- **Function:** Volume and softness.

### 3️⃣ Shadow 3: The Occlusion (Ambient Occlusion)
The darkest areas where ambient light does not reach.
- **Krita Tool:** `Basic-5 Size` (Low opacity) or `Multiply` layer mode.
- **Location:** Deep folds, contact points between objects (neck/shirt, hair/forehead).
- **Rule:** Occupies the least space but provides the most depth.

## Krita Workflow

1. **`Shadow 1` Layer (Multiply):** Paint geometric shadow shapes with hard edges.
2. **`Shadow 2` Layer (Overlay/Normal):** Use the Airbrush with a saturated/orange-ish color right on the terminator line (edge of Shadow 1) to create the "vibrant skin" effect.
3. **`Occlusion` Layer (Multiply):** Paint small, dark triangles at intersections (e.g., corners of the eyes, under the nose).

> [!example] Practical Example
> Imagine a sphere:
> 1. Hard shadow circle on the side opposite to the light.
> 2. Blur the edge towards the dark side, and add a saturated orange rim on the light/shadow transition.
> 3. Near-pure black exactly where the sphere touches the ground.

[[Week-02-Exercises]]
