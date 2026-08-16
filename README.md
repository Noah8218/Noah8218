<div align="center">

# Noah Choi (최노아)

### Machine Vision Software Engineer · C# / .NET / WPF

**2D/3D Inspection · Semiconductor Inspection · Automation Equipment · Vision Developer Tools**

[![GitHub](https://img.shields.io/badge/GitHub-Noah8218-181717?style=flat-square&logo=github)](https://github.com/Noah8218)
[![Email](https://img.shields.io/badge/Email-dhqtlzm12%40naver.com-03C75A?style=flat-square)](mailto:dhqtlzm12@naver.com)
[![Raw Buffer Visualizer](https://img.shields.io/visual-studio-marketplace/v/openvisionlab.RawBufferVisualizer?label=Raw%20Buffer%20Visualizer&style=flat-square)](https://marketplace.visualstudio.com/items?itemName=openvisionlab.RawBufferVisualizer)

</div>

---

## About Me

I am a **C#-based industrial machine-vision software engineer** focused on software that must run reliably on real automation equipment.

My work spans the full inspection workflow: **2D/3D vision, image processing and inspection algorithms, camera/light/motion/PLC integration, inspection sequences, result storage, logging, database integration, performance tuning, and field stabilization**.

I care especially about the parts that become critical in long-running equipment software: **deterministic state transitions, callback and thread safety, image-buffer lifetime, timeout/recovery paths, traceability, reproducibility, and diagnostics**.

> 산업용 머신비전과 자동화 설비를 위한 C#/.NET 소프트웨어를 개발합니다.  
> 알고리즘 구현뿐 아니라 장비에서 오래 안정적으로 동작하고, 문제가 발생했을 때 원인을 추적하고 복구할 수 있는 소프트웨어를 지향합니다.

---

## OpenVisionLab

**OpenVisionLab** is my open-source ecosystem for C# machine-vision developers.

The goal is to make it easier to **build, debug, validate, label, and simulate machine-vision workflows even when physical equipment is not immediately available**.

| Project | What it does | Status |
| --- | --- | --- |
| **[OpenVisionLab](https://github.com/Noah8218/OpenVisionLab)** | OpenCvSharp-based rule vision workbench for Layers, Tools, Pipelines, Recipes, Preview/Run, and Good/Bad validation | Public · Active |
| **[Raw Buffer Visualizer](https://github.com/Noah8218/RawBufferVisualizer)** | Visual Studio debugger tool for `Bitmap`, OpenCvSharp/Emgu `Mat`, `IntPtr`, raw buffers, camera wrappers, stride/format diagnostics, and image comparison | Public · Marketplace |
| **[OpenVisionLab Vision SDK](https://github.com/Noah8218/OpenVisionLab-Vision-SDK)** | UI-independent C# SDK for 2D inspection and height-map/full-XYZ 3D computation | Public |
| **[OpenVisionLab Labeling Studio](https://github.com/Noah8218/OpenVisionLab-Labeling-Studio)** | Windows workbench for object detection, segmentation, anomaly labeling, dataset management, training, validation, and model comparison | Public |
| **[OpenVisionLab 3D Studio](https://github.com/Noah8218/OpenVisionLab-3D-Studio)** | Rule-based 3D inspection workbench for height data, meshes, point clouds, ROI teaching, measurement, validation, and recipe replay | Public · Active |
| **OpenVisionLab Machine Studio** | Virtual-commissioning and equipment-simulation workbench for axes, I/O, devices, sequences, faults, conveyors, sensors, and virtual-camera workflows | In development |

### Ecosystem Direction

```text
Machine / Camera / Raw Buffer
        │
        ├── Raw Buffer Visualizer      → Debug buffers inside Visual Studio
        │
        ├── OpenVisionLab              → Build and validate 2D rule inspections
        │       └── Vision SDK         → Reusable 2D/3D inspection algorithms
        │
        ├── Labeling Studio            → Build datasets and validate AI models
        │
        ├── 3D Studio                  → Teach and validate 3D inspection recipes
        │
        └── Machine Studio             → Simulate equipment behavior before hardware is ready
```

---

## Featured Project — Raw Buffer Visualizer

**Image Watch-style debugging for C# and OpenCvSharp machine vision.**

Instead of repeatedly saving temporary images or writing debug-only conversion code, Raw Buffer Visualizer lets developers inspect image variables directly while stopped at a breakpoint.

[![Marketplace](https://img.shields.io/visual-studio-marketplace/v/openvisionlab.RawBufferVisualizer?label=Marketplace&style=flat-square)](https://marketplace.visualstudio.com/items?itemName=openvisionlab.RawBufferVisualizer)
[![Marketplace installs](https://img.shields.io/visual-studio-marketplace/i/openvisionlab.RawBufferVisualizer?style=flat-square)](https://marketplace.visualstudio.com/items?itemName=openvisionlab.RawBufferVisualizer)
[![GitHub stars](https://img.shields.io/github/stars/Noah8218/RawBufferVisualizer?style=flat-square&logo=github)](https://github.com/Noah8218/RawBufferVisualizer)

Key areas include:

- `System.Drawing.Bitmap`, OpenCvSharp `Mat`, Emgu CV `Mat`, `IntPtr`, and raw-buffer inspection
- Automatic inspection of supported image-like locals and arguments
- Buffer interpretation diagnostics for stride, pixel format, valid bits, and byte order
- A/B comparison, diff, blink, linked pan/zoom, line profile, histogram, and pixel inspection
- Large-image handling and fail-closed validation for unsafe or inconsistent buffer metadata

---

## Engineering Focus

- **Industrial Machine Vision** — 2D/3D inspection, image processing, measurement, matching, defect detection
- **Equipment Software** — inspection sequences, motion/PLC/camera/light integration, state management, timeout and recovery
- **C# Desktop** — WPF, WinForms, MVVM, async/multithreading, long-running application stability
- **Image Memory & Performance** — `Bitmap`, `BitmapSource`, OpenCvSharp `Mat`, `IntPtr`, camera callbacks, large-image ownership and lifetime
- **Traceability** — structured logs, inspection results, database/file persistence, reproducible diagnostics
- **Developer Tooling** — Visual Studio extensions, reusable vision SDKs, offline-capable engineering tools

---

## Tech Stack

<p>
  <img src="https://img.shields.io/badge/C%23-512BD4?style=flat-square&logo=dotnet&logoColor=white" alt="C#" />
  <img src="https://img.shields.io/badge/.NET-512BD4?style=flat-square&logo=dotnet&logoColor=white" alt=".NET" />
  <img src="https://img.shields.io/badge/WPF-0C54C2?style=flat-square&logo=windows&logoColor=white" alt="WPF" />
  <img src="https://img.shields.io/badge/WinForms-0C54C2?style=flat-square&logo=windows&logoColor=white" alt="WinForms" />
  <img src="https://img.shields.io/badge/OpenCV-5C3EE8?style=flat-square&logo=opencv&logoColor=white" alt="OpenCV" />
  <img src="https://img.shields.io/badge/OpenCvSharp-5C3EE8?style=flat-square&logo=opencv&logoColor=white" alt="OpenCvSharp" />
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/Visual%20Studio-5C2D91?style=flat-square&logo=visualstudio&logoColor=white" alt="Visual Studio" />
  <img src="https://img.shields.io/badge/Git-F05032?style=flat-square&logo=git&logoColor=white" alt="Git" />
  <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white" alt="GitHub Actions" />
</p>

---

## What I Value in Vision Software

```text
Correct inspection
    + predictable equipment behavior
    + safe image/buffer ownership
    + recoverable failures
    + useful logs and traceability
    + repeatable validation
    = software that can survive the production floor
```

I prefer practical engineering improvements that make a system **more stable, easier to diagnose, and easier to reproduce** over adding technology only for novelty.

---

<div align="center">

### Building practical machine-vision tools for C# developers.

**Machine Vision · Automation · Inspection · Developer Tools**

</div>
