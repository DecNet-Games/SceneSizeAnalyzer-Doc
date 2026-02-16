---
layout: default
title: Getting Started
nav_order: 3
permalink: /docs/getting-started
---

# Getting Started

## 1. Open the Scene Analyzer Window
In Unity, navigate to:
`Tools > Scene Size Analyzer > Object Density Manager`

(Note: The window name might vary slightly based on version, look for "Scene Analyzer" or "Object Density").

## 2. Prepare Your Project
Before running a scan, ensure your scenes are saved. The tool will open scenes in the background to analyze them.
> **Warning**: Always save your current open scene before starting a batch scan to avoid data loss.

## 3. Run a Scan
1. In the Scene Analyzer window, click **"Analyze Build Settings Scenes"** (or similar button depending on UI version).
2. The tool will iterate through all enabled scenes in your Build Settings.
3. Wait for the progress bar to complete.

## 4. Interpret Results
The dashboard will populate with a list of scenes. Key columns:
- **Scene Name**: Click to ping the scene asset.
- **Risk Level**: Color-coded (Green/Yellow/Red).
- **Object Count**: Total GameObjects.
- **Renderer Count**: MeshRenderers + SkinnedMeshRenderers.
- **Est. Size**: Predicted size of assets referenced in the scene.

## 5. View Details
Click on any row to open the **Scene Details Window**, which shows a breakdown of the heaviest assets in that specific scene.
