---
layout: post
title: Audio Reactive Stable Diffusion in Realtime
---

I used Olegchomp's [TouchDiffusion](https://github.com/olegchomp/TouchDiffusion) component in TouchDesigner to create a real-time audio-visual experience. This component allowed me to blend diffusion models with live audio input, generating captivating visuals that react in sync with the sound. The result is a dynamic, immersive visuals that showcases the power of combining generative art with real-time sound analysis.

<video controls>
  <source src="https://github-production-user-asset-6210df.s3.amazonaws.com/3389529/378226427-dc7205de-f073-4b97-bc35-78067aaf4913.webm?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAVCODYLSA53PQK4ZA%2F20241020%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20241020T213635Z&X-Amz-Expires=300&X-Amz-Signature=7220e5780eec199323a18113f1f9a0ae74d0a664b76aaf6ca0a59cc0ffd37c5d&X-Amz-SignedHeaders=host" type="video/webp">
</video>

The component utilizes img2img generation using [StreamDiffusion](https://github.com/cumulo-autumn/StreamDiffusion) to create real-time visuals based on an audio-reactive mask I developed. I've achieved impressive results with both SD-turbo and realisticVisionV60B1 + LCM.

![image](https://github.com/user-attachments/assets/aef76c54-54ce-4bc0-b4fb-46ad27ed5390)

This technology is truly exciting, with endless possibilities. The ability to update prompts in real-time and have visuals rendered in response to audio elevates stage performance to an entirely new level. I can't wait to showcase this in my upcoming performances!
