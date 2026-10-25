![Qyvaria Preview](https://i.imgur.com/KKOznyl.png)

![Image 1](https://i.imgur.com/cvGDrKi.png)

![Image 2](https://i.imgur.com/dwwtFCd.png)

![Image 3](https://i.imgur.com/0WyKUyw.png)

# Qyvaria OS & Computational Dimensional Shift Ecosystem

> **A Local-First, Browser-Native AI Operating Kernel and Multi-Axis State Transformation Engine**
> 
> **Primary Author & Architect:** John Havlasek  
> **Affiliation:** Qyvaria AI Systems & Cybernetics Group (Prague / Frýdek-Místek, Czech Republic)  
> **Core Runtime:** `qyvaria.py` (OnePy Fusion++)  
> **Classification:** Source-Grounded Technical Implementation & Research Specification  

---

## 📋 Overview

**Qyvaria** inverts the conventional OS-AI paradigm. Rather than treating Large Language Models (LLMs) and multi-agent frameworks as cloud-hosted API services, Qyvaria embeds runtime management, state synchronization, multi-agent orchestration, and context memory directly into a local-first, custom browser shell (`qyvaria://`) powered by a single-file Python microkernel (`qyvaria.py`).

The ecosystem implements **Computational Dimensional Shift (DS)**—a mathematical and architectural framework that enables continuous multi-axis state transformations across sandboxed execution timelines, dynamic hybrid logic engines, and continuous 3D behavioral manifolds without state snapping or network serialization overhead.

---

## 🏗️ Concentric 3-Layer Architecture

Qyvaria decouples execution logic from network backends through a three-layer concentric design:

```
+-----------------------------------------------------------------------+
|  Layer 3: Qyvaria OS (Visual Operating Shell)                         |
|  * Browser Shell (qyvaria://) | Workspace & Vault UX | Telemetry      |
+-----------------------------------------------------------------------+
        |
        v
+-----------------------------------------------------------------------+
|  Layer 2: AI Software & BIOS (Qyvaria Com)                            |
|  * Agent Orchestration | QyChat | Neural Graph State Mapping         |
+-----------------------------------------------------------------------+
        |
        v
+-----------------------------------------------------------------------+
|  Layer 1: Python Kernel (qyvaria.py Runtime Bridge)                    |
|  * Single-File OnePy Fusion++ | Local Model Bus (Ollama) | IPC        |
+-----------------------------------------------------------------------+
```

1. **Layer 1 — Python Kernel (`qyvaria.py` / OnePy Fusion++):** A self-contained, highly optimized single-file runtime wrapper using custom `MetaPathFinder` import hooks to execute virtualized modules in-memory without mandatory disk hits or cloud APIs.
2. **Layer 2 — AI BIOS & Orchestration (Qyvaria Com):** Low-level parameter tuning, multi-agent dispatching, contextual memory indexing via `BitWeaver`, and dynamic routing.
3. **Layer 3 — Visual Operating Shell (Qyvaria OS):** Cyber-aesthetic desktop workspace rendered natively, supporting dynamic module rails, reactive telemetry panels, and native `qyvaria://` protocol routing.

---

## 🌀 Computational Dimensional Shift (DS)

In Qyvaria, a **Dimensional Shift** refers to software state transformations across isolated execution contexts, processing paradigms, and multi-axis state coordinates.

### Mathematical Formalization

Instead of stepping abruptly between static state representations, the core engine maintains continuous linear/tensor interpolation across high-dimensional manifolds $S \in \mathbb{R}^D$ and low-precision execution target spaces $\Omega \in \mathbb{R}^d$:

$$\Psi(t) = (1 - \alpha(t)) \cdot Q(S_{\text{raw}}) + \alpha(t) \cdot T(S_{\text{compressed}}), \quad \alpha(t) \in [0, 1]$$

Where $\alpha(t)$ represents the continuous shift parameter evolving across system ticks, ensuring smooth gradient flow during lookahead evaluations and behavioral recalculations.

### The Three Operational Dimensions

| Dimension | Named Mechanism | Technical Operation | Rationale |
| :--- | :--- | :--- | :--- |
| **State-Space Partitioning** | **MetaSimAgent** | Dynamically forks active memory into volatile, sandboxed lookahead timelines. | Explores hypothetical agent scenarios without mutating baseline environment state. |
| **Paradigm Routing** | **OnePy / BitWeaver** | Dynamically routes tasks between classical $A^*$ symbolic rules, neural tensor models, and heuristics. | Adjusts solver logic in real time according to environmental entropy. |
| **Multi-Axis State Matrices** | **PAD Coordinate Engine** | Tracks behavioral state on a continuous 3D Pleasure-Arousal-Dominance (PAD) manifold. | Enables smooth trajectory scaling for AI policy and strategy decisions. |

---

## ⚡ Core Subsystems

* **`qyvaria.py` (OnePy Fusion++):** Bundles virtual modules (JSON payload containing SHA-256 verified inline Python source code). Overrides default import arrays (`find_spec`, `create_module`, `exec_module`) for dynamic in-memory injection.
* **`BitWeaver Core`:** Dynamic bit-stream interleaving and real-time entropy-based vector/context memory indexing engine.
* **`MetaSimAgent`:** Volatile simulation-of-simulations engine with `compile`, `run`, `traces`, `plan`, `fork_subsim`, and `snapshot` capabilities.
* **Deterministic Tool Engine:** Enforces static typing dry-runs and max VRAM limits prior to tool execution to eliminate state corruption.

---

## 📊 Comparative Architectural Matrix

| Architectural Vector | Legacy / Discrete Baseline | Qyvaria Continuous Model | Execution Advantage |
| :--- | :--- | :--- | :--- |
| **State Interpolation** | Discrete boolean flags; instant snaps causing context drop. | Continuous linear/tensor interpolation $\Psi(t)$ across ticks. | **Zero State Loss** |
| **Memory Sandbox** | Hard process forks; high RAM overhead & leaks. | `MetaSimAgent` volatile lookahead with non-mutating clones. | **Isolated & Volatile** |
| **Behavioral Axis** | Scalar threshold triggers; rigid rule checks. | Continuous 3D PAD manifold smooth scaling. | **Smooth Trajectory** |
| **Logic Routing** | Static switch/case routing; single-engine lock. | Dynamic `BitWeaver` + `OnePy` symbolic/neural hybrid engine. | **Adaptive Runtime** |
| **Dependency Footprint** | External cloud APIs and cloud vendor lock-in. | Self-contained in-memory bundle with custom import hook. | **100% Local / Self-Contained** |

---

## 🚀 Getting Started & Execution

### Bundle Management (`qyvaria.py`)

The single-file runtime acts as both an execution library and an orchestration entry point.

```bash
# List virtual modules embedded in the OnePy bundle
python3 qyvaria.py --list

# Extract virtual modules to disk for inspection
python3 qyvaria.py --extract ./extracted_modules

# Boot system entry point
python3 qyvaria.py --run
```

### Local Model Integration

Qyvaria routes requests locally to quantized models (e.g., Qwen3 family via Ollama):

* **Fast Interactive Lane (QChat):** `Qwen3:8b` (INT4, ~5.2 GB VRAM)
* **Deep Agent Orchestration:** `Qwen3:14b` (INT4, ~9.8 GB VRAM)
* **Dry-Run Code Synthesis:** `Qwen3:Coder-14b` (INT8, ~14.1 GB VRAM)
* **BitWeaver Memory Index:** Flat Vector (~0.8 GB VRAM)

---

## 🧪 Verification Protocol

To verify state isolation deterministically:
1. Record primary memory state SHA-256 hash before invoking a lookahead route.
2. Execute `MetaSimAgent.fork_subsim()`.
3. Verify that sandbox state mutates as intended while primary state hash remains identical.
4. Capture PAD vector coordinates and assert continuous gradient movement without sudden scalar jumps.

---

## 📄 License & Attribution

Designed, engineered, and authored by **John Havlasek**.  
All rights reserved under the **Qyvaria AI Systems & Cybernetics Group** research license.
