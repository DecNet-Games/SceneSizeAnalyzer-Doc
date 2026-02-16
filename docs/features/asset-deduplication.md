---
layout: default
title: Asset Deduplication
parent: Features
nav_order: 2
---

# Asset Deduplication Tool

It's common for developers to accidentally duplicate assets—like copying a texture to test something and forgetting to delete it. The Asset Deduplicator finds these files.

## How it Works
The tool calculates a hash for every asset in your project (specifically targeting Textures, Audio, and Meshes). If two files have the same content (even with different names), they are flagged.

## Using the Tool
1. Open `Tools > Scene Size Analyzer > Asset Deduplicator`.
2. Click **"Find Duplicates"**.
3. Review the groups of duplicate assets.
4. **Action**: Select the assets you want to keep and delete the duplicates. Update references in your scenes (pro-tip: use "Select Dependencies" in Unity to find usages).

## Performance Note
Hashing thousands of large textures can take a moment. The tool runs on a background thread where possible to keep the editor responsive, but large projects may experience a brief pause.
