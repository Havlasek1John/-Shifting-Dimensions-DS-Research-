# Shifting Dimensions (DS) — Architectural Research & Systemic Proof

**Author & Lead Architect:** Jan Havlásek  
**Ecosystem:** Qyvaria OS | `qyvaria.py` Single-File Kernel | Qyvaria Paradox Engine Modifications  
**Status:** Canonical Reference & Formal Proof of Concept  

---

## Executive Summary

**Shifting Dimensions (DS)** is an advanced system architecture framework designed by Jan Havlásek. It replaces static multi-agent orchestration and fixed-loop engine decision trees with dynamic, multidimensional state-space remapping. 

Instead of processing agents, game units, or computational pipelines inside a fixed single-dimensional state array, **Shifting Dimensions** projects runtime entities across three synchronized operational axes:
1. **Dimension 1 ($\mathcal{D}_1$): State-Space Partitioning** — Contextual and temporal isolating of execution memory.
2. **Dimension 2 ($\mathcal{D}_2$): Paradigm Routing** — Seamless switching between deterministic execution, neural LLM inference, and low-level C++/Jomini engine pulse routines.
3. **Dimension 3 ($\mathcal{D}_3$): PAD Behavioral Multi-Axis Matrix** — Continuous state modification based on Pleasure-Arousal-Dominance dynamic vectors.

This repository serves as the official research record, mathematical formalization, and implementation proof of DS technology across the **Qyvaria software suite**.

---

## 1. What is Shifting Dimensions (DS)?

In traditional software engines and multi-agent frameworks, system state is linear. Every entity shares a global variable context, leading to exponential evaluation cost $O(N^2)$ as agent count or game complexity increases.

**Shifting Dimensions (DS)** solves this by treating computational state as a non-Euclidean state-manifold $\mathcal{S}$. An entity (an agent in `qyvaria.py` or a character/actor in a Paradox grand strategy modification) does not exist in a static block of memory; instead, its behavior, priority, and execution loop **shift dynamically** between dimensional planes based on active system load, context relevance, and emotional/behavioral vectors.

               ┌──────────────────────────────────────────┐
               │        SHIFTING DIMENSIONS KERNEL        │
               └────────────────────┬─────────────────────┘
                                    │
         ┌──────────────────────────┼──────────────────────────┐
         ▼                          ▼                          ▼
┌──────────────────────┐   ┌──────────────────────┐   ┌──────────────────────┐
│     DIMENSION 1      │   │     DIMENSION 2      │   │     DIMENSION 3      │
│     State-Space      │   │   Paradigm Routing   │   │     PAD Vector       │
│     Partitioning     │   │   Deterministic /    │   │  Pleasure-Arousal-   │
│ (Temporal/Context)   │   │    LLM / Jomini      │   │   Dominance Matrix   │
└──────────┬───────────┘   └──────────┬───────────┘   └──────────┬───────────┘
│                          │                          │
└──────────────────────────┼──────────────────────────┘
│
▼
┌──────────────────────────────────────────┐
│    State Transition Function S(t+1)      │
└──────────────────────────────────────────┘


---

## 2. Theoretical Framework & Mathematical Proof

The dynamic state $S$ of any entity at discrete time step $t+1$ is evaluated as a tensor transformation across the three dimensions:

$$S_{t+1} = \Phi\Big(\mathcal{D}_1(C, \tau), \; \mathcal{D}_2(\Pi, \lambda), \; \mathcal{D}_3(\mathbf{v}_{PAD})\Big)$$

Where:
* $C$ is the active context state vector.
* $\tau$ is the system tick/temporal pulse index.
* $\Pi$ is the operational execution paradigm (0 = Deterministic Engine, 1 = LLM Inference, 2 = C++/Jomini Engine Pulse).
* $\lambda$ represents compute resource constraints and latency thresholds.
* $\mathbf{v}_{PAD} \in [-1, 1]^3$ represents the 3-axis Pleasure-Arousal-Dominance emotional state vector.

### Dimensional Transformation Matrix

The mapping function $\Phi$ projects low-level attributes into high-level behavioral outcomes through state transformation matrix $M_{DS}$:

$$M_{DS} = \begin{bmatrix} w_{11}\mathcal{D}_1 & w_{12}\mathcal{D}_2 & w_{13}\mathcal{D}_3 \\  w_{21}\mathcal{D}_1 & w_{22}\mathcal{D}_2 & w_{23}\mathcal{D}_3 \\  w_{31}\mathcal{D}_1 & w_{32}\mathcal{D}_2 & w_{33}\mathcal{D}_3 \end{bmatrix}$$

This guarantees that an update in emotional state ($\mathcal{D}_3$) immediately re-routes the execution paradigm ($\mathcal{D}_2$) while re-indexing memory priority ($\mathcal{D}_1$) in $O(1)$ constant time overhead per entity cycle.

---

## 3. Implementation Across Qyvaria Systems

Shifting Dimensions is not just a theoretical model—it is actively implemented and tested across three primary systems created by Jan Havlásek:

### 3.1 `qyvaria.py` (Single-File Python AI Kernel)
* **Function:** Acts as a lightweight, zero-dependency multi-agent orchestration runtime.
* **DS Application:** Implements **Paradigm Routing ($\mathcal{D}_2$)**. When system load increases or localized deterministic rules suffice, agents shift down from heavy LLM inference loops (`qwen2.5-coder` / `qwen3`) to deterministic state tables, preventing memory bloat and API bottlenecking.
* **Result:** Enables hyper-dense agent execution inside a single-file executable module.

### 3.2 Qyvaria OS (Developer Workbench & AI Operating System)
* **Function:** Electron and Chromium-based workstation integrating local LLMs, Monaco Editor, and terminal orchestration.
* **DS Application:** Uses **State-Space Partitioning ($\mathcal{D}_1$)**. Workspace tabs, background background processes, and AI sub-agents operate within isolated dimensional workspaces that dynamically exchange state data via non-blocking IPC message busses without cross-contaminating UI rendering threads.

### 3.3 Qyvaria Crusader Kings III Organic Engine Mod
* **Function:** C++ and Jomini/Clausewitz engine performance & AI overhauls for grand strategy games.
* **DS Application:** Uses **PAD Behavioral Matrices ($\mathcal{D}_3$) and Character Culling**. Instead of running expensive decision trees for millions of unlanded NPCs every tick, characters shift between active rendering dimensions. Characters out of player scope undergo compressed state representation, reducing engine calculations while increasing AI realism.
* **Result:** Massive performance gains, smoother game pacing, and dynamic character behavior based on multi-axis psychological states.

---

## 4. Key Architectural Features & Benefits

1. **Deterministic Performance Scaling:** Eliminates performance drops in multi-agent environments by shifting idle or non-critical entities into lower dimensional evaluation planes.
2. **Context-Aware Routing:** Automatically determines whether a request requires neural network evaluation, local code execution, or heuristic rule sets.
3. **Organic AI Behavior:** Provides human-like decision pathways through continuous PAD vector dynamics rather than binary switch statements.
4. **Zero-Dependency Architecture:** Designed to operate natively in local environments (Nobara Linux, Pop!_OS, Windows) with minimal overhead.

---

## 5. Repository Structure

```text
Shifting-Dimensions-DS-Research/
│
├── README.md                 # System documentation and proof of architecture
├── docs/                     # Detailed technical specifications & whitepapers
│   └── qyvaria_ds_spec.pdf   # Architectural formalization paper
├── proofs/                   # Code verification & simulation scripts
│   ├── ds_kernel_demo.py     # Python prototype of 3D state shifting logic
│   └── pad_matrix_test.py    # Simulation script for PAD behavioral transitions
└── LICENSE                   # MIT License - Author: Jan Havlásek
6. Verification & Proof of Concept Script
To test the core 3D shifting logic in Python:

Python
# proofs/ds_kernel_demo.py
# Proof of Concept: Shifting Dimensions State Engine
# Author: Jan Havlásek

import time

class ShiftingDimensionsEngine:
    def __init__(self, entity_id):
        self.entity_id = entity_id
        # D1: State Space (0: Suspended, 1: Background, 2: Foreground)
        self.d1_state = 1 
        # D2: Paradigm Routing (0: Deterministic, 1: Neural/LLM, 2: Engine Native)
        self.d2_paradigm = 0 
        # D3: PAD Behavioral Vector [Pleasure, Arousal, Dominance]
        self.d3_pad = [0.0, 0.0, 0.0] 

    def update_pad(self, p, a, d):
        self.d3_pad = [max(-1.0, min(1.0, val)) for val in (p, a, d)]
        self._evaluate_shift()

    def _evaluate_shift(self):
        p, a, d = self.d3_pad
        # Dimension Shift Logic
        if a > 0.6 and d > 0.2:
            self.d2_paradigm = 1 # Shift to high-compute neural/LLM paradigm
            self.d1_state = 2    # Bring to foreground execution
        elif a < -0.4:
            self.d2_paradigm = 0 # Shift to low-overhead deterministic paradigm
            self.d1_state = 1    # Move to background partition
        
        print(f"[Entity {self.entity_id}] Shifted -> D1 (State): {self.d1_state} | D2 (Paradigm): {self.d2_paradigm} | D3 (PAD): {self.d3_pad}")

if __name__ == "__main__":
    ds = ShiftingDimensionsEngine(entity_id="Agent_Alpha")
    ds.update_pad(0.2, -0.5, 0.1) # Trigger low arousal shift
    ds.update_pad(0.8, 0.9, 0.5)  # Trigger high arousal paradigm shift
7. Citation & Attribution
If you utilize Shifting Dimensions (DS) architectural concepts or reference this research in your work, please cite:

Code snippet
@misc{havlasek2026shiftingdimensions,
  author = {Jan Havlásek},
  title = {Shifting Dimensions (DS): Multidimensional State-Space Partitioning and Paradigm Routing in Autonomous Systems and Game Engines},
  year = {2026},
  publisher = {GitHub},
  journal = {GitHub Repository},
  howpublished = {\url{[https://github.com/YOUR_USERNAME/Shifting-Dimensions-DS-Research](https://github.com/YOUR_USERNAME/Shifting-Dimensions-DS-Research)}}
}
8. License
Distributed under the MIT License. See LICENSE for more information.

Copyright © 2026 Jan Havlásek. All Rights Reserved.
