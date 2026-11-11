<div align="center">

# Shayan Muhammad
### Senior Agentic Systems Engineer & Product Architect

<p align="center">
  <b>Full Product Stakeholder • Zero-Trust Agentic Architectures • Upstream Open-Source Contributor</b><br/>
  Driving systems from zero-to-one: from formal architectural specifications and adversarial audit reports to production-grade deployment.
</p>

[![GitHub](https://img.shields.io/badge/GitHub-ShayanMuhammad--CS-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/ShayanMuhammad-CS)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Shayan%20Muhammad-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/shayan-muhammad-cs)
[![Email](https://img.shields.io/badge/Email-shayanmuhammad.cs%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:shayanmuhammad.cs@gmail.com)

</div>

---

```yaml
Profile: Full-Stack Product Architect & Senior AI Systems Engineer
Operating Mode: Sole Stakeholder (End-to-End Ownership: Concept → Spec → Audit → Build → Deploy)
Core Disciplines: Deterministic Agent Guardrails · Local Air-Gapped RAG · Multimodal Vision · Distributed Systems
Engineering Philosophy: Code-level mathematical guarantees over probabilistic LLM assumptions
```

---

## 🏛️ Systems & Products (Full Stakeholder Ownership)

*These are systems where I own the complete lifecycle as the sole stakeholder: product strategy, formal system specifications (EGM), adversarial audit reports, and production code.*

### 1. [Shaheen & IntentLock™](https://github.com/ShayanMuhammad-CS/hunter) — Zero-Trust Agentic Execution & Escrow
* **Role**: Product Lead & Principal Architect (End-to-End Stakeholder)
* **The Problem**: Autonomous AI agents suffer from the "Checkout Cliff"—hallucinating orders, violating budget bounds, and remaining susceptible to stealth prompt-injections during live checkout.
* **The Architecture**:
  * **Cryptographic Intent Invariants**: Compiles raw user intents into mathematically bounded Pydantic schemas.
  * **Two-Phase Financial Escrow**: Integrates PayPal Sandbox v2 (`AUTHORIZE` $\rightarrow$ `CAPTURE`). Funds are placed on programmatic hold; capture is strictly gated behind zero-trust validation.
  * **Deterministic Runtime Guardrails**: Enforces code-level interceptors (`guardrails.py`) that prevent agent self-modification or test tampering, combined with Chrome DevTools Protocol (CDP) Shadow DOM traversal.
  * **Audit Reports & Specs**: Built via the Elephant-Goldfish Model (EGM), documented through exhaustive formal design specifications and independent adversarial audit reports.

### 2. [Multimodal RAG Pipeline](https://github.com/ShayanMuhammad-CS/Multimodal_RAG_Pipeline) — Document Intelligence Engine
* **Role**: System Architect & Developer
* **The Architecture**: Pairs dense vector retrieval with Vision-Language Models (VLMs) to process documents containing complex tabular figures, charts, and diagrams without information loss from lossy OCR/caption extraction.

### 3. [DocuMind](https://github.com/ShayanMuhammad-CS/DOCUMIND-RAG-for-Your-Notes) — Air-Gapped Local Neural RAG
* **Role**: System Architect & Developer
* **The Architecture**: A zero-telemetry, fully local personal knowledge engine powered by ChromaDB, Ollama, and cross-encoder reranking. Guarantees 100% data residency with zero external API dependencies.

### 4. [MeetSense](https://github.com/ShayanMuhammad-CS/MeetSense) — Modular Audio Intelligence
* **Role**: System Architect & Developer
* **The Architecture**: Real-time audio/video ingest, diarization, speech-to-text, and conversational intelligence pipeline engineered for high-noise acoustic environments.

### 5. [DeforestAI](https://github.com/ShayanMuhammad-CS/DEFORESTAI-DETECTION-SYSTEM) — Satellite Vision Monitoring
* **Role**: Machine Learning Engineer & Lead
* **The Architecture**: Computer vision segmentation network processing multi-spectral satellite imagery to identify and monitor deforestation dynamics over temporal datasets.

---

## 🚀 Internal Product & Production Engineering Work

Beyond standalone public repositories, I have driven and delivered **15+ production feature sets** across team codebases and internal platforms:
* **Kanban & State Management**: Architected multi-lane interactive Kanban boards with real-time state synchronization, drag-and-drop mechanics, and optimistic UI updates.
* **Per-User View State & Preferences**: Built persistence layers for customized filtering, sorting layouts, and saved workspace configurations.
* **Permission Scoping & RBAC**: Implemented role-based access control engines, tenant isolation boundaries, and cryptographic route guards.
* **Secure Attachment Pipelines**: Engineered authenticated file download streams, virus scanning hooks, and presigned asset delivery.
* **Accessibility (a11y) Conformance**: Refactored complex component trees for full WCAG/ARIA compliance, keyboard navigation focus rings, and screen-reader tree semantics.

---

## 🌐 Upstream Open Source Contributions (Major Ecosystem Repos)

*Direct technical contributions and architectural patches to widely adopted open-source frameworks:*

| Major Repository | Contribution & Subsystem | Status |
| :--- | :--- | :---: |
| [**modelcontextprotocol / servers**](https://github.com/modelcontextprotocol/servers) | **Model Context Protocol (MCP) Server Confinement & Isolation**<br/>Engineered boundary and repository scope isolation configurations for `mcp-server-git`, hardening unconfined tool execution parameters for agentic context pipelines. | `Contributions` 🛡️ |
| [**adbar / trafilatura**](https://github.com/adbar/trafilatura) | **High-Fidelity Web & DOM Extraction Engine**<br/>Contributed robust text discovery, document structure parsing, and DOM edge-case filtering routines powering downstream LLM ingestion pipelines. | `Contributions` ⚡ |
| [**huggingface / smolagents**](https://github.com/huggingface/smolagents/pull/2755) | **CPython Argument Binding in Local Python Executor**<br/>Engineered standard CPython keyword/positional argument resolution for tool calling in local sandboxes. Resolved critical parameter mapping mismatches during autonomous agent execution. | `PR Shipped` 🚀 |
| [**makenotion / notion-sdk-js**](https://github.com/makenotion/notion-sdk-js/pull/779) | **Block Schema & Column Nesting Validation**<br/>Fixed child block nesting constraints allowing `column_list` and `column` structures inside single-level-nestable parent blocks across official JavaScript SDK typings. | `PR Shipped` 🚀 |
| [**refined-github / refined-github**](https://github.com/refined-github/refined-github/pull/10013) | **Deployment Visibility & Status Filtering**<br/>Extended `hide-inactive-deployments` to intelligently prune failed and stale deployment markers across dense enterprise GitHub dashboards, improving workflow visibility for thousands of developers worldwide. | `Merged` ✅ |
| [**tscircuit / schematic-symbols**](https://github.com/tscircuit/schematic-symbols/pull/452) | **Hardware EDA Symbol Specifications**<br/>Contributed standardized phototransistor optical schematic symbol geometry and pin definitions for the open-source browser EDA circuit ecosystem. | `PR Shipped` 🚀 |

---

## 📋 Architectural Rigor: Reports & EGM Spec Methodology

Every production system I lead is developed using the **Elephant-Goldfish Model (EGM)**, ensuring design decisions are rigorously documented and stress-tested before implementation:

* **Concept Briefs (`docs/briefs/`)**: High-level problem formulation, checkout cliff dynamics, and ROI analysis.
* **Formal System Specifications (`docs/designs/`)**: Mathematical invariant definitions, Pydantic bounds, and two-phase sequence diagrams.
* **Adversarial Audit Reports (`docs/reviews/`)**: Zero-context adversarial evaluations checking for prompt injection vulnerabilities, state drift, and race conditions.
* **Deterministic Ground-Truth Evals (`evals/`)**: Python-based test suites validating invariant compliance and zero-trust policies under adversarial stress.

---

## 💻 Technical Capabilities

<div align="center">

| Area | Technologies & Methods |
| :--- | :--- |
| **Languages** | `Python (AsyncIO, AST, CPython Internals)` · `TypeScript` · `JavaScript` · `SQL` · `Bash` |
| **Agentic & AI** | `LiteLLM` · `LangChain` · `SmolAgents` · `Ollama` · `ChromaDB` · `Cross-Encoders` · `VLMs` |
| **Systems & Backend** | `FastAPI` · `Node.js` · `PostgreSQL` · `Redis` · `Docker` · `Chrome DevTools Protocol (CDP)` |
| **Frontend & UI** | `React 19` · `Next.js` · `TailwindCSS` · `Gradio` · `Vite` |
| **Architecture** | `EGM Spec-Driven Development` · `Zero-Trust Verification` · `AST Interceptors` · `CI/CD Evals` |

</div>

---

## 📊 GitHub Analytics

<div align="center">

<img height="155" src="https://github-readme-stats.vercel.app/api?username=ShayanMuhammad-CS&show_icons=true&theme=github_dark&hide_border=true&bg_color=0D1117&icon_color=58A6FF&title_color=58A6FF&text_color=8B949E" alt="GitHub Stats" />
<img height="155" src="https://github-readme-stats.vercel.app/api/top-langs/?username=ShayanMuhammad-CS&layout=compact&langs_count=6&theme=github_dark&hide_border=true&bg_color=0D1117&title_color=58A6FF&text_color=8B949E" alt="Top Languages" />

<br/>

<img src="https://github-readme-streak-stats.herokuapp.com/?user=ShayanMuhammad-CS&theme=github-dark-blue&hide_border=true&background=0D1117" alt="GitHub Streak" />

</div>

---

<div align="center">
  <sub>Engineered with deterministic rigor by <b>Shayan Muhammad</b> • <a href="mailto:shayanmuhammad.cs@gmail.com">shayanmuhammad.cs@gmail.com</a></sub>
</div>
