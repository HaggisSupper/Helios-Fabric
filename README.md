# Helios Fabric (v1.1.4)

**Local-First Hybrid LLM Orchestration Fabric**

Helios Fabric is a deterministic, local-first orchestration layer designed to leverage all available compute (GPU, CPU, iGPU) on Windows 11 environments.

## Core Philosophy
- **Determinism > Autonomy**: Explicit routing rules over LLM self-decision.
- **Local-First**: Persistent RAG and memory using LanceDB.
- **Cloud Bursting**: Controlled access to OpenRouter for heavy tasks.
- **Windows Native**: Optimized for Windows 11 DTE, using WSL2 only for compute.

## Tech Stack
- **Language**: Python 3.12
- **Package Manager**: [uv](https://github.com/astral-sh/uv) (Strictly no `requirements.txt`)
- **API**: FastAPI
- **Database**: LanceDB (Vector/Memory)

## Getting Started
1. Install `uv`.
2. Run `uv sync` to install dependencies and create the lockfile.
3. Start the orchestrator: `uv run main.py` (Implementation in progress).