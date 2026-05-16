---
layout: post
title: "SD-orb: Building a Real-time AI VJ Orchestrator"
---

The intersection of generative AI and live performance is a chaotic, beautiful frontier. For years, VJs (Visual Disk Jockeys) have used recursive feedback loops and audio-reactive shaders to create hypnotic textures. With the advent of Stable Diffusion, we can now inject high-level semantic imagination into these loops.

Today, I’m releasing **SD-orb**, a real-time AI VJ orchestrator designed to push the boundaries of what's possible in a live setting.

### The Problem: Latency
Stable Diffusion is powerful, but it’s historically slow. In a VJ context, "slow" is the enemy. If your visuals don't respond to the kick drum instantly, the immersion is broken. To solve this, SD-orb leverages **NVIDIA TensorRT 10** and **LCM (Latent Consistency Models)**.

### The Performance
On an RTX 4090, SD-orb achieves staggering results:
- **UNet Inference**: ~8ms (compared to ~45ms in PyTorch)
- **End-to-End Pipeline**: ~12ms
- **Output**: A fluid 80+ FPS at 512x512 resolution.

This isn't just "fast for AI"; it's fast enough for real-time recursive feedback.

### The Recursive Feedback Engine
SD-orb doesn't just generate static images. It uses a custom `Visualizer` that applies warp, zoom, and rotation transformations to the *previous* AI-generated frame before feeding it back into the next step. 

When you map the bass frequencies to the zoom factor and the mids to the rotation, the AI begins to "dance." The prompt (e.g., *"cinematic portrait, realistic lighting, 8k"*) acts as the lens through which this feedback loop is viewed, creating a constantly evolving, dream-like stream of consciousness.

### Tech Stack
- **Engine**: TensorRT 10 (compiled via StreamDiffusion patterns)
- **Model**: Realistic Vision V6.0 B1 + LCM LoRA
- **Reactivity**: PyAudio (FFT analysis)
- **UI**: DearPyGui (for real-time parameter tweaking)
- **Graphics**: Pygame-CE (for the feedback math)

### Open Source
I’ve released the source code, installation guide, and performance metrics on GitHub. You can find everything you need to build your own engine and start performing here:

[**GitHub: xaymup/SD-orb**](https://github.com/xaymup/SD-orb)

This is just the beginning of what I want to do with "Recursive AI." The ghost in the shell is starting to move to the beat.
