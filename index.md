---
layout: home
title: Home
nav_order: 1
---

# Scene Size Analyzer
{: .fs-9 }

Stop optimizing blindly. Get instant insights into your Unity scenes.
{: .fs-6 .fw-300 }

[Get Started](./docs/getting-started.html){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }
[View on GitHub](https://github.com/DecNet-Games/SceneSizeAnalyzer-Doc){: .btn .fs-5 .mb-4 .mb-md-0 }

---

## What is Scene Size Analyzer?

Scene Size Analyzer is a powerful **Editor-only** tool designed to help Unity developers visualize and reduce the memory footprint of their scenes. 

Instead of guessing why your build size is large or why a scene takes forever to load, get a detailed breakdown of object counts, renderer density, and asset duplication risks.

## Key Features

### 🔍 Deep Scene Analysis
Scan your entire project or specific scenes to get metrics on:
- **Object Count**: Total GameObjects in the scene.
- **Renderer Count**: Number of active renderers (Meshes, Skinned Meshes).
- **Disk Size**: Estimated build size of the scene assets.

### ♻️ Asset Deduplication
Identify duplicated assets (Textures, Meshes, Audio) that are wasting precious disk space. Our smart hashing algorithm finds identical files even if they have different names.

### 🤖 CI/CD Automation
Integrate performance checks into your build pipeline. The **Headless Scanner** runs in batch mode, analyzes scenes, and can fail the build if risk thresholds are exceeded.

### 🔥 Visualization
Use the **Scene Heatmap** to visually identify areas with high object density directly in the Scene View.

---

## Why use it?

| **Pain Point** | **Solution** |
|:---|:---|
| "My APK/IPA size is too big!" | Pinpoint the exact scenes and assets contributing to the bloat. |
| "This level runs slow on mobile." | Identify high renderer counts and object density instantly. |
| "We have duplicate textures everywhere." | Find and consolidate duplicates with the Asset Deduplicator. |
| "Did we break performance limits?" | run automated checks in your CI pipeline. |

---

## Installation

Ready to optimize?

[Install Now](./docs/getting-started.html){: .btn .btn-blue }
