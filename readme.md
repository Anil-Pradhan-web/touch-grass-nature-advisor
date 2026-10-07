# touch-grass-nature-advisor
# 🌿 Touch Grass AI: Edge Expedition Planner

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/Anil-Pradhan-web/touch-grass-nature-advisor/blob/main/touch_grass_ai.ipynb)
[![License: Apache 2.0](https://img.shields.io/badge/License-Apache_2.0-blue.svg)](LICENSE)
[![Hacktoberfest 2026](https://img.shields.io/badge/Hacktoberfest-2026-orange.svg)](https://hacktoberfest.com)
[![Model: Google Gemma 2](https://img.shields.io/badge/Model-Gemma--2--2B--IT-green.svg)](https://huggingface.co/google/gemma-2-2b-it)

An offline-first, edge-ready outdoor expedition companion engineered to disconnect software professionals from screen fatigue. Built with **Google Gemma 2 (2B)**, deterministic physics-based trail telemetry, and strict **Pydantic** structured schema validation.

---

## 📌 Architecture Overview

Traditional lifestyle and outdoor AI applications depend on cloud APIs, which fail on remote alpine trails without cellular reception. **Touch Grass AI** operates as a hybrid edge pipeline:

1. **Deterministic Telemetry Engine:** Computes real-time solar elevation angles and atmospheric lapse rate adjustments locally using pure mathematical heuristics.
2. **Open-Weight Reasoning Core:** Evaluates computed risks using Google's open-weight `gemma-2-2b-it` model running on-device via Hugging Face Transformers.
3. **Structured Verification Gate:** Enforces deterministic JSON compliance via Pydantic schemas, eliminating generative hallucination.

```text
[ User Activity & GPS / Altitude ]
                │
                ▼
┌────────────────────────────────────────┐
│   OfflineEnvironmentEngine             │
│   • Solar Elevation Approximation      │
│   • Altitude Lapse Rate (-6.5°C/1km)   │
└──────────────────┬─────────────────────┘
                   │ Telemetry Vectors
                   ▼
┌────────────────────────────────────────┐
│   Gemma-2-2B-IT Edge LLM               │
│   • Contextual Outdoor Synthesis       │
│   • Screen-Free Protocol Generation    │
└──────────────────┬─────────────────────┘
                   │ Raw Generation
                   ▼
┌────────────────────────────────────────┐
│   Pydantic Schema Validation           │
│   • OutdoorPlanSchema Contract Gate    │
└──────────────────┬─────────────────────┘
                   │
                   ▼
[ Validated Expedition Dispatch (JSON) ]
