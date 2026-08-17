<div align="center">

# Noah Choi

### Industrial Machine Vision Software Engineer

**C# · .NET · WPF · 2D/3D Vision · Automation Equipment · Developer Tools**

[![GitHub](https://img.shields.io/badge/GitHub-Noah8218-181717?style=flat-square&logo=github)](https://github.com/Noah8218)
[![Email](https://img.shields.io/badge/Email-dhqtlzm12%40naver.com-03C75A?style=flat-square)](mailto:dhqtlzm12@naver.com)
[![Raw Buffer Visualizer](https://img.shields.io/visual-studio-marketplace/v/openvisionlab.RawBufferVisualizer?label=Raw%20Buffer%20Visualizer&style=flat-square)](https://marketplace.visualstudio.com/items?itemName=openvisionlab.RawBufferVisualizer)

**Building open-source tools for machine-vision development before the physical machine is ready.**

</div>

---

## About

I am an industrial machine-vision software engineer with **8 years of experience across 20+ equipment projects** in semiconductor, display, battery, and automotive manufacturing.

My professional work covers the complete equipment-software lifecycle: requirements, software architecture, inspection implementation, equipment integration, validation, production deployment, and field stabilization.

My personal R&D focuses on a recurring problem I have seen in real equipment development:

> **When software development starts only after the machine and samples are ready, validation risk is concentrated near the end of the schedule.**

I am building **OpenVisionLab** to move more of that work earlier by connecting virtual equipment, image data, inspection software, reusable algorithms, and validation workflows.

---

# OpenVisionLab

**OpenVisionLab is my personal open-source R&D ecosystem for C# machine-vision developers.**

The long-term goal is to provide a reusable environment where small vision teams and individual developers can design, implement, debug, and validate inspection software even when access to production equipment is limited.

## Project Family

### [OpenVisionLab — 2D Inspection Workbench](https://github.com/Noah8218/OpenVisionLab)

A Windows desktop workbench for building and validating **rule-based 2D machine-vision inspections** with OpenCvSharp.

- Layer-based image workflow
- Threshold, Filter, Morphology, Blob, Contour, Matching, Line and measurement tools
- Ordered inspection Pipelines and reusable Recipes
- Intermediate-image review and explicit Preview / Run behavior
- Good / Bad sample validation
- Public sample workflows designed for reproducibility

**Status:** Public · Active development · Public sample validation

---

### [OpenVisionLab Vision SDK](https://github.com/Noah8218/OpenVisionLab-Vision-SDK)

The shared inspection core behind the OpenVisionLab project family.

- UI-independent C# inspection libraries
- 2D image-processing and inspection algorithms
- Height-map and full-XYZ 3D computation
- Thickness, Warpage, Flatness, Gap/Flush, Volume and geometry operations
- Shared coordinate, measurement, result and data contracts
- Designed so UI applications can reuse the same inspection logic without duplicating algorithms

**Status:** SDK 3.0 source public · Used by OpenVisionLab

---

### [OpenVisionLab Labeling Studio](https://github.com/Noah8218/OpenVisionLab-Labeling-Studio)

A Windows desktop workbench for building and validating machine-vision AI datasets.

- Object detection, segmentation and anomaly labeling
- Dataset versioning and validation
- Training workflow integration
- Candidate-model review and comparison
- Shared ground-truth data across supported model adapters
- Explicit separation between labels, AI candidates and adopted inspection models

**Status:** Public · Core workflow implemented

---

### [OpenVisionLab 3D Studio](https://github.com/Noah8218/OpenVisionLab-3D-Studio)

A rule-based 3D inspection workbench for teaching, measurement, validation and recipe replay.

- Height Map, mesh and point-cloud workflows
- ROI teaching and inspection-step configuration
- Thickness and Warpage inspection
- Plane, gap, flush, volume and geometry measurements
- Preview, Publish, Run and validation workflows
- Repeatable recipe and evidence review

**Status:** Public · Thickness / Warpage validation in progress

---

### OpenVisionLab Machine Studio

A virtual-commissioning workbench for validating equipment behavior before physical equipment is available.

Current implementation includes:

- Equipment layout, Sequence and Recipe concepts
- Axis, I/O, Sensor and deterministic simulation
- Automatic cycle execution
- Fault Injection and timeout/recovery scenarios
- Virtual Camera and Image Source timing
- Inspection Cell concepts for connecting vision software

The next integration stage connects the OpenVisionLab project family so simulated camera acquisition can drive 2D, 3D and AI inspection workflows and return inspection results to the equipment sequence.

**Status:** Core simulation implemented · Inspection integration in progress

---

## OpenVisionLab Direction

```text
Equipment Concept / Process Design
            │
            ▼
     Machine Studio
  Sequence · Axis · I/O · Fault
            │
            ▼
 Virtual Camera / Image Source
            │
     ┌──────┼─────────────┐
     ▼      ▼             ▼
 2D Vision  3D Vision     AI Data / Validation
OpenVision  3D Studio     Labeling Studio
     │      │             │
     └──────┴──────┬──────┘
                   ▼
          OpenVisionLab Vision SDK
                   │
                   ▼
       Inspection Result / Metrics
                   │
                   ▼
         Sequence Decision / Replay
```

The purpose is not to replace real equipment validation. It is to **move architecture, sequence, inspection, failure-mode and integration verification earlier**, so physical-machine time can be used for the things that truly require hardware, optics and production samples.

---

# Raw Buffer Visualizer

### [Visual Studio Marketplace](https://marketplace.visualstudio.com/items?itemName=openvisionlab.RawBufferVisualizer) · [GitHub](https://github.com/Noah8218/RawBufferVisualizer)

**Raw Buffer Visualizer** is a separate developer tool created from the debugging problems I repeatedly encountered while developing C# machine-vision software.

Instead of saving temporary images or writing debug-only conversion code, it allows image and raw-buffer variables to be inspected directly while stopped at a breakpoint in Visual Studio.

[![Marketplace](https://img.shields.io/visual-studio-marketplace/v/openvisionlab.RawBufferVisualizer?label=Marketplace&style=flat-square)](https://marketplace.visualstudio.com/items?itemName=openvisionlab.RawBufferVisualizer)
[![Marketplace installs](https://img.shields.io/visual-studio-marketplace/i/openvisionlab.RawBufferVisualizer?style=flat-square)](https://marketplace.visualstudio.com/items?itemName=openvisionlab.RawBufferVisualizer)
[![GitHub stars](https://img.shields.io/github/stars/Noah8218/RawBufferVisualizer?style=flat-square&logo=github)](https://github.com/Noah8218/RawBufferVisualizer)

Key areas include:

- `System.Drawing.Bitmap`, OpenCvSharp `Mat`, Emgu CV `Mat`, `IntPtr` and raw buffers
- Debugger visualizers and automatic image-like object inspection
- Stride, pixel-format, valid-bit and byte-order diagnostics
- Buffer interpretation recovery for incorrectly described raw images
- Pixel inspection, histogram, line profile and image comparison
- A/B, split, diff, blink and linked pan/zoom workflows
- Large-image handling and fail-closed buffer validation

**Status:** Marketplace release · v2.0.2

---

## Experience Behind the Projects

These personal projects are based on problems I have handled in production machine-vision systems rather than isolated demo applications.

### Machine Vision

- 2D: Edge, Blob, Contour, Pattern Matching, Line Gauge and measurement
- 3D: Height Map, Full XYZ, Thickness and Warpage
- Image coordinate conversion, defect merging and inspection-result processing
- Area Scan and Line Scan camera workflows

### Equipment Software

- Camera, lighting, I/O, sensor, PLC and motion integration
- Inspection Sequence and Recipe architecture
- TOP / BTM independent processing and multi-worker execution
- Timeout, recovery and delayed-callback isolation
- Long-running equipment-state and error-handling design

### Performance & Interop

- C++ DLL / C++/CLI / C# interoperability
- Large unmanaged image buffers
- Multi-threaded inspection queues
- Rule / AI inspection-module integration
- Native / managed boundary design

### Desktop & Tooling

- C# / .NET
- WPF / WinForms
- OpenCvSharp
- Visual Studio extensions
- Git / SVN / Jenkins / GitHub Actions

---

## Engineering Principles

```text
Build earlier.
Validate explicitly.
Keep state deterministic.
Fail safely.
Preserve evidence.
Make problems reproducible.
```

I prefer engineering that improves **stability, traceability, recovery and reproducibility** over adding complexity only for novelty.

For machine-vision software, an algorithm producing the right result once is not enough. The complete system must acquire the correct image, execute the correct inspection at the correct time, preserve the result, recover from failure, and provide enough evidence to explain what happened later.

---

<div align="center">

### Open-source machine-vision tools built from production equipment experience.

**C# · .NET · Machine Vision · Automation · 2D/3D Inspection · Developer Tools**

</div>
