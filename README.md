# The_IFG_Idea
Open and lightweight "visual DNA" system for image generation using parametric fractals and semantic AI prompts. A possible competitor to AI image generators, more efficient and without losing quality.

# The IFG Idea — Intelligent Fractal Generator

> ⚡ A radically lightweight, explainable, and open system for generating images through parametric fractals, modular semantics, and controllable randomness. Think: **visual DNA meets prompt-based generation**.

---

## 🎯 Pitch

Modern image generators like Stable Diffusion, Midjourney, or DALL·E are powerful — but they require:

- Huge gigabyte-scale neural weights,
- Expensive GPUs for slow inference,
- Unpredictable generations with poor modularity,
- Little to no semantic explainability.

The **IFG (Intelligent Fractal Generator)** is a radically different vision:

> A generation system where images are constructed from **semantic fractal components** — like visual genes — controlled by a **tiny semantic AI**, rendered through **parametric equations**, and optionally randomized with **seed-based variability**.

---

## 🧬 What is a `.frac` file?

A `.frac` is a **modular visual gene**: a JSON-based structure that describes a single element — like a dog’s ear, a human eye, or a tree branch — using:

- A **mathematical equation** (Bezier, L-System, Superformula, IFS, etc.),
- A set of **adjustable parameters** (scale, curvature, color, symmetry...),
- **Anchor points** for semantic/structural attachment,
- Tags for **semantic meaning** (e.g. `["eye", "female", "elf"]`),
- Optional **rendering hints** (style, color, material).

These components are like building blocks for image assembly.

---

## 🧠 The Lightweight AI

A small embedded AI module interprets natural language prompts and:

- Parses semantic meaning,
- Selects appropriate `.frac` components,
- Adjusts parameters contextually,
- Applies controlled randomness using **seed-based variation**.

This AI can be implemented using lightweight NLP methods or even rule-based systems, making it feasible for offline or embedded use.

---

## 🧪 Controlled Randomness with Seeds

Every generation can use a seed:

- The **same prompt + same seed** yields **the same result**,
- A **different seed** allows variation in proportions, component choices, and visual style,
- Parameters in `.frac` files can allow **bounded mutation**, e.g.:

```json
"curvature": {
  "base": 0.4,
  "delta_max": 0.1,
  "seed_dependent": true
}
