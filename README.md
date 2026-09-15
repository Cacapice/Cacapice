# Hello, thanks for stopping by 👋

### Mathematical foundations, observability, and validation for autonomous AI systems

I build tools for understanding **what AI agents did, why they did it, and whether their behavior can be trusted**.

My work combines **statistical inference, mathematical modeling, provenance, and software engineering** to make autonomous systems more observable and auditable.

Rather than treating AI evaluation as a collection of pass/fail tests, I'm interested in systems where **uncertainty is quantified, behavior is measurable, evidence is preserved, and claims about reliability can be independently examined**.

---

## 🔬 Current Work

My work focuses on three related problems:

**AI Validation**
Developing empirical methods for evaluating autonomous-agent behavior and detecting unexpected, unstable, or unsupported behavior.

**Statistical & Geometric Analysis**
Investigating how optimization, parameterization, Fisher information, sampling, and other mathematical structures affect conclusions drawn about learned systems.

**Agent Provenance & Observability**
Building infrastructure that records agent actions and state transitions so behavior can be reconstructed, analyzed, and audited.

---

## 🚀 Featured Work

My projects approach reliable AI from two complementary directions: **the mathematical foundations of valid inference and the infrastructure required to preserve evidence about autonomous systems.**

### 🧮 Theory — [Inferential Fidelity Framework](https://github.com/Cacapice/Inferential-Fidelity-Framework)

**A framework for reasoning about whether transformations preserve the evidence required for downstream inference.**

The project explores the relationship between representation, information preservation, and the validity of conclusions drawn from transformed data.

Its central concern is not simply whether two representations appear similar, but whether the transformation preserves the information necessary to support the inference being made.

**Research themes:**

* Inferential validity
* Evidence preservation
* Statistical information
* Representation and transformation
* Mathematical AI validation

[Explore Inferential Fidelity Framework →](https://github.com/Cacapice/Inferential-Fidelity-Framework)

---

### ⚙️ Infrastructure — [AgentLedger](https://github.com/Cacapice/AgentLedger)

**An evidence and observability layer for autonomous AI agents.**

AgentLedger records agent operations as structured, auditable events so developers can reconstruct what an agent did and analyze its behavior programmatically.

The project is evolving toward a safety-oriented infrastructure component for agent systems, with features including:

* **Atomic transactions** using Python context managers
* **Idempotency protection** against duplicate agent actions
* **Strict-mode controls** and operational guardrails
* **Structured event logging**
* **Pydantic-based validation**
* **Pandas / CSV export** for analysis
* **Programmatic spending limits**
* **Automated testing and CI**

```python
with ledger.transaction():
    ledger.debit("research_agent", 10)
    ledger.credit("analysis_agent", 10)
```

Agent retries can be made idempotent:

```python
ledger.debit(
    "research_agent",
    10,
    idempotency_key="task_2026_001"
)
```

The objective is straightforward:

> Give autonomous systems an evidence trail that can be inspected, tested, and independently verified.

[Explore AgentLedger →](https://github.com/Cacapice/AgentLedger)

---

## 🔭 Research

### Bayesian Inference

Using posterior updating and uncertainty quantification to evaluate evidence about model and agent behavior.

### Fisher Information & Optimization

Studying whether observed properties of learned systems are intrinsic to the learned function or artifacts of **parameterization, optimization, sampling, or measurement**.

This includes investigating Fisher information spectra, optimizer-dependent behavior, identifiability, and the distinction between properties of a learned function and properties of its coordinate representation.

### Formal Operational Boundaries

Exploring mathematical representations of allowable agent states and transitions as a foundation for enforceable behavioral constraints.

### Provenance

Creating verifiable chains of evidence connecting **agent actions, state transitions, policies, observations, and resulting claims**.

---

## 🧭 From Theory to Systems

My work follows a common progression:

**Mathematical foundations**
↓
What information is required to justify an inference?

**Measurement & empirical validation**
↓
Can that information be reliably observed and quantified?

**Evidence infrastructure**
↓
Can the relevant actions, states, and observations be preserved?

**Autonomous systems**
↓
Can agent behavior be reconstructed, tested, and audited?

The goal is to connect mathematical questions about **what can legitimately be inferred** with engineering systems that preserve the evidence needed to answer those questions.

---

## 🛠️ Technical Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge\&logo=python\&logoColor=white)
![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge\&logo=numpy\&logoColor=white)
![PyMC](https://img.shields.io/badge/PyMC-Probabilistic_Programming-blue?style=for-the-badge)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge\&logo=postgresql\&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge\&logo=docker\&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge\&logo=githubactions\&logoColor=white)

---

## 🧭 Engineering Philosophy

Reliable autonomous systems require more than successful outputs.

They require infrastructure capable of answering:

1. **What happened?**
2. **What evidence produced the decision?**
3. **What changed between runs?**
4. **Was the action inside its permitted operating boundary?**
5. **What uncertainty accompanies the result?**
6. **Can the result be reproduced or independently audited?**

A system should not merely produce an answer. It should preserve enough evidence for that answer—and the process that produced it—to be examined.

---

## 📊 GitHub

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=Cacapice\&show_icons=true\&include_all_commits=true\&count_private=true)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=Cacapice\&layout=compact\&langs_count=7)

---

## 📬 Connect

I'm interested in collaborations around **agent infrastructure, AI validation, probabilistic modeling, interpretability, statistical inference, and reliable autonomous systems**.

[GitHub](https://github.com/Cacapice) · [X](https://twitter.com/Cacapice) · [LinkedIn](https://www.linkedin.com/in/kjombrellaro/)
