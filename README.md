<p align="center">
  <img src="logo.svg" alt="Contract Negotiation Logo" width="128" height="128" />
</p>

<h1 align="center">Contract Negotiation</h1>

> **Reinforcement Learning Environment for AI-Driven Legal Contract Review and Strategic Negotiation**

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python)](https://python.org)
[![OpenEnv](https://img.shields.io/badge/OpenEnv-Compatible-brightgreen)](https://github.com/meta-llama/openenv)
[![Docker](https://img.shields.io/badge/Docker-Ready-2496ED?logo=docker)](https://docs.docker.com/)
[![Pytest](https://img.shields.io/badge/Tests-Passing-success?logo=pytest)](https://docs.pytest.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow)](https://opensource.org/licenses/MIT)

Contract Negotiation is an OpenEnv reinforcement learning environment where an AI agent acts as an autonomous legal reviewer. The agent inspects procedural contract drafts, detects hidden unfair clauses and liability traps, exchanges redlines with an adversarial or heuristic counterparty, and sequentially decides whether to accept, propose amendments, or walk away.

## Tech Stack

- **Environment:** OpenEnv, Gymnasium interface, Procedural Contract Generation
- **Evaluation & Grading:** Automated legal trap scoring, amendment fairness metrics, rubric grading
- **Agent Policies:** Risk-aware negotiator, tit-for-tat heuristic, learned counterpolicies
- **Infrastructure:** Docker, Python 3.10+, Pytest

## Key Features

- **Procedural Contract Generation:** Dynamic NDAs, SaaS SLAs, and vendor service agreements with randomized clauses and hidden traps.
- **Multi-Turn Negotiation Loop:** Strategic counter-proposals with fairness tracking, concession bounds, and round limits.
- **Objective Rubric Scoring:** Quantitative evaluation on trap detection rate, amendment precision, deal fairness, and walk-away accuracy.
- **Plug-and-Play Policy Evaluation:** Benchmark baseline rule-based policies against advanced LLM legal reviewers.

## Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/ankitgpt18/Contract-Negotiation.git
   cd Contract-Negotiation
   ```

2. **Environment Setup**
   Create a virtual environment and install dependencies:
   ```bash
   python -m venv .venv
   # Windows: .venv\Scripts\activate
   # Unix: source .venv/bin/activate
   pip install -r requirements.txt
   ```

3. **Run Interactive Demo**
   Execute a simulated multi-turn contract negotiation session:
   ```bash
   python demo_run.py
   ```

4. **Run Strategy Showcase**
   Demonstrate targeted risk-aware counterparty evaluation:
   ```bash
   python showcase_run.py
   ```

5. **Run Tests and Benchmark**
   Execute test suites and generate benchmark report artifacts:
   ```bash
   python run_all.py
   ```

## Repository Structure

- `contract_negotiation_env/`: Core OpenEnv environment, models, policies, and procedural generators.
- `tests/`: Automated unit and integration test suites.
- `artifacts/`: Generated benchmark summaries and evaluation metrics.
- `demo_run.py`: Interactive CLI demonstration.
- `showcase_run.py`: Targeted risk-aware counterparty run.
- `run_all.py`: End-to-end benchmark and test runner.
- `SUBMISSION.md`: Detailed environment design and evaluation framework writeup.
- `RESULTS.md`: Empirical benchmark performance across contract types.
- `DEPLOYMENT.md`: Container build and deployment guide.

## License

This project is licensed under the MIT License.
