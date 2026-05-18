---
title: "Unity Voxel Engine #0: Series Introduction"
date: 2026-05-17T22:08:04+02:00
draft: false
description: "Kicking off a series on building a voxel engine in Unity from scratch, covering Binary Greedy Meshing, flood lighting, Ambient Occlusion, and custom physics."
summary: "Kicking off a series on building a voxel engine in Unity from scratch, covering Binary Greedy Meshing, flood lighting, Ambient Occlusion, and custom physics."
tags: ["unity", "voxels", "gamedev", "binary-greedy-meshing", "rendering"]
---

Ever since my adventure with gamedev began, voxels were always my favorite subject. Vast open worlds with infinite possibilities kept teasing my curiosity: how is it all made? How do games like Minecraft render enormous chunks of terrain without grinding to a halt?

{{< video src="preview.mp4" autoplay="true" loop="true" muted="true" controls="false" preload="auto" >}}

That question sent me down a long rabbit hole.

After watching [this fantastic talk on Greedy Meshing](https://www.youtube.com/watch?v=4xs66m1Of4A) by Davis Morley I got hooked on exploring yet another voxel engine implementation, this time using **Binary Greedy Meshing**. The idea is elegant: instead of processing faces one by one, you use bitwise operations to merge them in bulk, dramatically reducing the number of triangles needed to represent a chunk.

So I built one. And then I rebuilt it. And now I want to explain it.

## What This Series Is About

This series walks through my Unity voxel engine implementation step by step. I already have working source code, and the semi-final state is available [on this repo](https://github.com/Seremonik/Unity-Voxel-Engine). Rather than just publishing the code and calling it a day, I want to reconstruct it from scratch here, explaining the reasoning behind each decision along the way.

The final result of this series might differ slightly from the existing repo. Rebuilding from scratch often reveals better approaches.

## What You Should Know Going In

This is not a beginner series. I will assume you are comfortable with:

- **Unity's Job System**, for scheduling and running multithreaded work safely
- **Unity's Mesh API**, for constructing meshes at runtime via `Mesh` and `MeshDataArray`

I won't spend time explaining those fundamentals. The focus here is entirely on the voxel engine itself: chunk management, face culling, and the Binary Greedy Meshing algorithm.

If you need a refresher on Jobs or the Mesh API, Unity's own documentation and Turbo Makes Games' tutorials are solid starting points.

## What We're Building

By the end of this series we'll have a working voxel engine with:

- Infinite-ish world chunked into fixed-size regions
- Per-chunk mesh generation using Binary Greedy Meshing
- Multithreaded chunk building via the Job System
- Flood light algorithm
- Ambient Occlusion implementation
- Custom physics

## Up Next

The next post dives into the foundation: chunk data structures and how we represent the voxel world in memory.

Follow the newsletter below to get notified when it drops.
