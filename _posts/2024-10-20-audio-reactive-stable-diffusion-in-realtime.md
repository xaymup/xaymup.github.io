---
layout: post
title: Audio Reactive Stable Diffusion in Realtime
---

I used Olegchomp's [TouchDiffusion](https://github.com/olegchomp/TouchDiffusion) component in TouchDesigner to create a real-time audio-visual experience. This component allowed me to blend diffusion models with live audio input, generating captivating visuals that react in sync with the sound. The result is a dynamic, immersive visuals that showcases the power of combining generative art with real-time sound analysis.

<video controls>
  <source src="../video1.webp" type="video/webp">
</video>

The component utilizes img2img generation using [StreamDiffusion](https://github.com/cumulo-autumn/StreamDiffusion) to create real-time visuals based on an audio-reactive mask I developed. I've achieved impressive results with both SD-turbo and realisticVisionV60B1 + LCM.

![image](https://github.com/user-attachments/assets/aef76c54-54ce-4bc0-b4fb-46ad27ed5390)

This technology is truly exciting, with endless possibilities. The ability to update prompts in real-time and have visuals rendered in response to audio elevates stage performance to an entirely new level. I can't wait to showcase this in my upcoming performances!
