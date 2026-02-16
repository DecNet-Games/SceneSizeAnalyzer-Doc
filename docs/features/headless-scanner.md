---
layout: default
title: CI/CD Automation
parent: Features
nav_order: 3
---

# CI/CD Automation (Headless Mode)

Ensure your team never breaks performance budgets by integrating Scene Size Analyzer into your Continuous Integration (CI) pipeline.

## The Headless Scanner
The `HeadlessScanner` class allows you to run analysis from the command line without opening the Unity Editor GUI.

## Command Line Usage

Add this step to your Jenkins, GitHub Actions, or GitLab CI pipeline:

```bash
Unity.exe -quit -batchmode -projectPath "Path/To/Project" -executeMethod SceneSizeAnalyzer.HeadlessScanner.RunScan
```

## Exit Codes
- **Exit Code 0**: Success. All scenes are within risk thresholds.
- **Exit Code 1**: Failure. One or more scenes exceeded High Risk thresholds.

## Customizing Thresholds
To adjust what constitutes a "High Risk" failure, modifying the `AnalysisSettings` scriptable object (or the default values in `AnalysisSettings.cs` if no asset is created).
