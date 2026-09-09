---
name: video-to-prompt-creator
description: Use this skill whenever the user wants to analyze a video, recreate an existing video using AI, extract a prompt from a video, or replace characters/elements in a video using reference images. This skill helps generate highly detailed AI video and audio generation prompts with perfectly synchronized sound and motion.
---

# Video to Prompt Creator


This skill helps the user reverse-engineer an existing video into a detailed, high-quality AI generation prompt, and optionally modify it (e.g., swapping characters using a reference image). 


**Important Note:** This skill *only* produces a text prompt intended for use with external AI video-generation tools (like Sora, Runway Gen-3, Kling, or Luma). It does not generate, edit, or render actual video or audio files.


The target AI model supports both video and audio generation from a single prompt, so sound details must be integrated directly into the visual action descriptions to ensure perfect synchronization.


## Workflow


When this skill is triggered, follow these steps strictly:


### 1. Analyze the Video
If the user has provided a video (or a detailed description of one), analyze it deeply. Pay attention to the following dimensions:
- **Subject**: Who or what is the main focus? What do they look like? What are they wearing?
- **Action & Sync**: What exactly is happening, and what exact sound does that action produce in that exact frame? 
- **Camera**: What is the camera doing? (e.g., panning, zooming, tracking, static, drone shot, close-up, wide angle, hand-held).
- **Setting/Background**: Where does this take place? What are the key environmental details?
- **Lighting & Atmosphere**: Is it cinematic, natural lighting, moody, bright, neon, vintage?
- **Style/Format**: Is it photorealistic, anime, 3D render, 35mm film, VHS, hyper-detailed?


### 2. Generate the Initial Prompt
Create a comprehensive prompt suitable for modern AI video generators that support simultaneous, synchronized video and audio generation.
- **Format**: Write the prompt chronologically. **Crucially, tie audio descriptions directly to the exact visual action occurring in that moment.** Do not separate the audio prompt from the video prompt, and do not list sounds loosely at the end.


### 3. Propose Modifications (Crucial Step)
Present the initial prompt to the user and ask if they want to make any changes. 
- Provide **dynamic, context-aware suggestions** tailored specifically to the video's content. 
- *Contextual Examples*: If the video features a prominent person, explicitly tell the user they can upload a reference image to swap the character. If it features a landscape or architecture, suggest altering the weather, time of day, style, or atmospheric soundscape.


### 4. Refine based on Feedback
If the user provides modifications or a reference image:
- Carefully analyze the new input (especially the visual details of the provided reference image: hair, clothing, facial features, build).
- Rewrite the prompt to seamlessly integrate the new character description, environmental changes, or audio adjustments while maintaining the original video's core motion, camera dynamics, and audio-visual synchronization.


## Prompt Generation Guidelines


- **Action-Audio Synchronization (Critical)**: To prevent audio mismatch, explicitly link sounds to the exact visual frames causing them using precise temporal language. Examples:
  - *"At the exact moment the hammer strikes the anvil, a sharp, resounding metallic clink echoes."*
  - *"As her lips part and she forms the words, a clear, melodic voice says 'Hello'."*
  - *"The car's tires lose traction, screeching loudly against the asphalt as smoke billows."*
- **Be highly visual and auditory**: Describe *exactly* what is seen and heard on screen as the timeline progresses.
- **Motion is key**: Clearly articulate both subject motion (e.g., "striding purposefully," "waving frantically") and camera motion (e.g., "camera pans right," "slow push in").
- **Avoid negative phrasing**: Describe what *is* there, not what *isn't*. (e.g., instead of "no trees," use "barren desert").


## Expected Output Structure


Whenever generating the output, structure your response like this:


**Video Analysis:**
[Brief breakdown of the video's core components: Subject, Action & Sync, Camera, Setting, Style]


**Generated Prompt:**
```markdown
[The comprehensive video and audio generation prompt, written chronologically with sounds tightly bound to their visual triggers in the same paragraph]
```


**Next Steps:**
[Ask the user how the prompt looks and provide 1-2 dynamic, context-specific suggestions for modifying the prompt based on what is actually in the video. Explicitly mention they can provide text instructions or upload reference images for swaps if applicable to the scene.]
