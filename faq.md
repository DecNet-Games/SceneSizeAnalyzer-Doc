---
layout: default
title: FAQ
nav_order: 5
permalink: /faq
---

# Frequently Asked Questions

## Q: Does this tool modify my scenes?
**A:** No. The analysis is read-only. However, to scan scenes that are not currently open, the tool must open them in the Editor. It attempts to restore your original scene afterwards, but we always require saving your work before running a batch scan.

## Q: Why is the "Estimated Size" different from my final build size?
**A:** The "Estimated Size" sums the imported size of assets referenced in the scene. It does **not** account for:
- Asset Bundle stripping.
- Engine code stripping.
- Build compression (LZ4/LZMA).
- Assets shared between multiple scenes (each scene counts the full size of its dependencies).
Think of it as a "relative weight" metric rather than an exact byte count.

## Q: Can I run this at runtime?
**A:** No. This is an Editor-only tool (`#if UNITY_EDITOR`). It is designed to be stripped from the build to have zero runtime performance impact.

## Q: How do I ignore specific folders?
**A:** Currently, the scanner checks all scenes in `Build Settings`. To ignore a scene, remove it from the Build Settings or disable it. Future versions will support a `.ignore` config file.
