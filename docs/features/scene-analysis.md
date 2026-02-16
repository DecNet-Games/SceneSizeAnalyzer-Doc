---
layout: default
title: Scene Analysis
parent: Features
nav_order: 1
---

# Scene Analysis Dashboard

The core of the tool is the Scene Analysis Dashboard. It provides a high-level view of your project's strictness against performance budgets.

## Dashboard Columns

### Risk Level
The risk is calculated based on `AnalysisSettings`. Default limits (configurable):
- **Low Risk**: < 50k Objects, < 500k Triangles
- **Medium Risk**: < 100k Objects, < 1M Triangles
- **High Risk**: Exceeds above limits.

### Object Count
The total number of GameObjects in the scene hierarchy. High object counts increase CPU overhead due to transform updates.

### Renderer Count
The number of active `MeshRenderer`, `SkinnedMeshRenderer`, and `SpriteRenderer` components. This directly impacts draw calls and GPU load.

### Estimated Size
This is an **estimation** of the build size contribution of the scene. It sums the imported size of all assets (Textures, Models, Audio) referenced by the scene.
> **Note**: This does not account for asset sharing between scenes (unless you use the dedicated Build Report tool) or Asset Bundles.

## Actions
- **Ping**: Highlights the scene file in the Project view.
- **Open**: Opens the scene additively for inspection.
- **Details**: Opens a detailed breakdown of assets within the scene.
