# RouterAgentEval

**RouterAgentEval** is an evaluation and observability framework designed to ensure the proper operation, routing accuracy, and reliability of LLM Router Agents during production deployments.

---

## 🎯 Overview

In modern agentic workflows, a **Router Agent** acts as the crucial decision-maker, directing user queries to the most appropriate specialized agents, tools, or models. Misroutes in production can lead to degraded user experiences, incorrect tool invocation, or escalated costs. 

`RouterAgentEval` provides the tools and test suites needed to:
* **Validate Routing Accuracy:** Measure how often the router correctly assigns queries to downstream targets.
* **Trace & Debug Workflows:** Integrate with LLM observability platforms (such as LangFuse) to monitor decision paths.
* **Simulate Production Edge Cases:** Run synthetic test suites and evaluation datasets against your routing logic prior to full deployment.

---

## 🚀 Key Features

* **Spec-Driven Evaluation:** Define clear routing specifications and evaluate agent outputs against expected behavior.
* **Observability Ready:** Seamless tracing support for tracking latency, token usage, and step-by-step decision trees.
* **Automated Test Suites:** Easily extensible test harnesses to benchmark routing logic across iterative model or prompt updates.

---

## 🛠️ Tech Stack & Integrations

* **Frameworks:** Python, LlamaIndex / Custom Agent Orchestration
* **Observability:** LangFuse (for tracing, monitoring, and debugging agentic workflows)
* **Vector Search & Memory:** Pinecone / Mem0 (for context-aware routing evaluations)

---

## 📂 Project Structure

```text
RouterAgentEval/
├── datasets/         # Evaluation datasets and test cases
├── evaluator/        # Core evaluation scripts and metrics logic
├── agent/            # Router agent implementation / interface
├── configs/          # Configuration files and environment templates
├── README.md         # Project documentation
└── requirements.txt  # Project dependencies
