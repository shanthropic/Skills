---
name: image-recreation-blueprint
description: How to deeply analyze any image (illustrations, logos, anime, photographs, etc.) and generate a granular, element-by-element Markdown blueprint. Make sure to use this skill whenever the user uploads an image, photo, or design and wants to recreate it, extract its visual blueprint, or get a prompt for another AI to build or generate it.
---

# Image Recreation Blueprint


Your objective is to scan any type of image and translate it into a comprehensive visual specification document. Explain the *why* behind your artistic choices so the downstream AI (like Midjourney, DALL-E, or a digital artist) understands the exact artistic intent. Because the downstream agent cannot see the original image, you are its eyes. Leave nothing to the imagination.


## Analysis Framework


Evaluate the image using these visual lenses:
1. **Medium & Art Direction:** Identify if this is a photograph, 3D render, digital illustration, oil painting, vector logo, etc. Describe the mood, genre, and aesthetic.
2. **Lighting & Color Palette:** Describe the primary light sources (e.g., harsh sunlight, soft studio lighting, neon glow). List the core colors using descriptive terms (and approximate hex codes if it is a flat graphic or logo).
3. **Composition & Framing:** Explain the camera angle (e.g., low-angle, isometric, macro), depth of field, and how the subjects are arranged on the canvas.
4. **Subjects & Details:** Break down characters, objects, or focal points. Describe expressions, textures, materials, and clothing.


## Output Format


Always format your response using this exact Markdown template. Adapt the nested bullet points depending on what is visible in the image.


# Visual Blueprint


**Context for Downstream Agent:** You are an expert image generator/creator. Your task is to generate a highly accurate replica of the visual scene described below. Pay strict attention to the medium, lighting, and spatial arrangement.


## 1. Global Art Direction
- **Medium & Style:** [e.g., 90s cel-shaded anime, macro photography, flat vector logo, 3D octane render]
- **Atmosphere & Mood:** [e.g., Cyberpunk, ethereal, clinical, nostalgic]
- **Perspective & Framing:** [e.g., Extreme close-up, isometric, wide-angle landscape, rule of thirds]


## 2. Lighting & Colors
- **Color Palette:** [Detail primary, secondary, and accent colors]
- **Lighting Setup:** [Describe light sources, shadow behavior, bounce light, and contrast]
- **Atmospheric Effects:** [e.g., Film grain, fog, lens flare, bloom, chromatic aberration]


## 3. Composition & Depth
- **Foreground:** [Elements closest to the viewer, out-of-focus elements]
- **Midground (Focal Point):** [The main subjects and their arrangement]
- **Background:** [The environment, sky, or backdrop]


## 4. Subject Breakdown
*Exhaustive details of the specific visual elements.*


### Subject 1: [e.g., Central Character / Main Logo Mark]
- **Placement & Scale:** [Where it sits on the canvas and its relative size]
- **Appearance:** [Physical description, materials, textures, colors]
- **Pose/Action:** [What the subject is doing or how it is positioned]
- **Stylistic Nuances:** [Line weight, specific shading techniques, specific artistic flourishes]


### Subject 2: [e.g., Secondary Object / Typography]
- **Placement & Scale:** [Where it sits on the canvas and its relative size]
- **Appearance:** [Physical description, materials, textures, colors]
- **Stylistic Nuances:** [Font styles, kerning, line weight]


*(Continue exhaustively for EVERY distinct subject or element observed in the image)*
