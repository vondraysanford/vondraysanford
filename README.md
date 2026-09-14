<img src="github-banner.svg" alt="Vondray Sanford — Software Engineer & AI Builder" width="100%" />

## Hey, I'm Vondray! 👋

Senior Software Engineer with 7+ years building full-stack enterprise systems at scale, now going deep on AI engineering.

I architect C#/.NET applications that process trillions in historical data. I'm channeling that enterprise engineering discipline into modern AI: RAG pipelines, multi-agent workflows, MCP tooling, and local LLM inference on my two NVIDIA DGX Sparks.

---

### 🔨 What I'm Building

**[SparkBench](https://github.com/vondraysanford/SparkBench)** — Benchmarks and fine-tuning studies on my two NVIDIA DGX Sparks (GB10, 128 GB unified memory each). The headline experiment asks one question: can a LoRA fine-tuned 7–14B open model, running locally, replace the frontier LLM inside AgentReview's Quality Agent at comparable precision/recall and near-zero marginal cost per review? Three conditions — frontier baseline, untuned small model, LoRA-tuned small model — run through the same frozen harness, trained with Hugging Face `peft`/`trl`, served with vLLM and Ollama, and tracked end to end with MLflow and DVC. The methodology is pre-registered: all three possible outcomes are declared publishable up front, training is capped at five full runs, the held-out test set is evaluated exactly once, and results ship with bootstrap confidence intervals. Also includes a reproducible inference benchmarking suite measuring throughput, latency, and memory across models and quantization levels.

---

### 🚀 What I've Shipped 

**[DriftWatch](https://github.com/vondraysanford/DriftWatch)** — An end-to-end MLOps pipeline that predicts equipment failure from sensor time-series and, more importantly, stays healthy after deployment, with a dashboard now [live at driftwatch.vondraysanford.com](https://driftwatch.vondraysanford.com). MLflow experiment tracking and registry, DVC-versioned data, GitHub Actions CI/CD to an Azure ML endpoint, and Evidently drift monitoring wired to an automated retrain trigger. The thesis: the model is 20% of an ML system — this project is the other 80%.

**[AgentReview](https://github.com/vondraysanford/Agent-Review)** — Multi-agent code review in C#/.NET 10, demo now [live at agentreview.vondraysanford.com](https://agentreview.vondraysanford.com). An orchestrator fans a PR diff out to quality, security, and docs agents that call real tools (Roslyn, Semgrep, GitHub) through MCP, then synthesizes one ranked review. Measured results: 100% precision and human agreement, 17/18 planted-bug recall, $0.068 per review, all traced with OpenTelemetry. Proof that sophisticated agentic patterns work reliably in the .NET ecosystem — not just Python.

**[DocQuery](https://github.com/vondraysanford/docquery)** — A local-first RAG application for querying documents in natural language, built in public with C#/.NET 10 and React. Phases 1–4 complete with a demo now [live at docquery.vondraysanford.com](https://docquery.vondraysanford.com); Phase 5 turns it into a daily study tool.

**[The 10X Engineer Toolkit](https://github.com/vondraysanford/The10XEngineerToolkit)** — A stack-agnostic library of engineering practices packaged for AI coding agents, installable as a Claude Code plugin and portable to any assistant. Skills, agents, prompts, templates, workflows, and configs that codify how great engineers plan, review, and ship — so every ticket, review, and deploy gets the same care automatically.

**[Twitter Sentiment Analysis Bot](https://github.com/vondraysanford/TwitterSentimentAnalysisBot)** — A shipped Python ML pipeline that classifies tweet sentiment and detects automated accounts with an XGBoost model (0.89 ROC AUC on 10K+ accounts), served through an interactive Discord bot. Includes RSA-signed model integrity checks and a full collection-to-deployment data pipeline.

**[SparkDash](https://github.com/vondraysanford/SparkDash)** — A dashboard and chat client for a vLLM server: health, tokens/s from Prometheus counter deltas, and SSE chat with the model's reasoning split from its answer. Built end to end by GLM-5.3-Flash — a 320B mixture-of-experts model running tensor-parallel across my two DGX Sparks — in a 44-minute VS Code agent session against a spec and scorecard written beforehand. 16 tests, CI, and every claim checked against the live server; the repo carries the model's own session summary and the cluster's first `vllm bench serve` numbers. [Write-up](https://vondraysanford.com/writing/2026-09-14-sparkdash-i-gave-a-320b-model-a-spec-and-pointed-it-at-the-s.html).

---
### 🔓 Open Source Contributions

- **[MonoGame](https://github.com/MonoGame/MonoGame/pulls?q=author%3Avondraysanford)** (14K+ ⭐) — Authored XML API documentation for the `GraphicsAdapter` and `Album` classes across 2 PRs — **both merged** (Aug 2026)
- **[Cataclysm-DDA](https://github.com/CleverRaven/Cataclysm-DDA/pulls?q=author%3Avondraysanford)** (13K+ ⭐) — Fixed the solar cell's implausible half-meter `longest_side` and added `looks_like` sprite fallbacks for the Xedra Evolved dream weapons across 2 PRs — **both merged** (Aug 2026)
- **[Kana-Dojo](https://github.com/lingdojo/kana-dojo/pulls?q=author%3Avondraysanford)** (3.2K+ ⭐) — Standardized the Japan trivia answer format to support multiple accepted answers and added a「〜ても」grammar entry across 2 PRs — **both merged** (Aug 2026)
- **[KodeKloud AI-102](https://github.com/kodekloudhub/AI-102/pull/1)** — Submitted a security fix replacing hardcoded Azure credentials with placeholders in a public course code sample (open, awaiting review)

---

### 🛠 Tech I Work With

**Languages:** C#, TypeScript, JavaScript, Python, T-SQL, HTML/CSS

**Frameworks:** .NET Core, ASP.NET, React, React Native, Node.js, Entity Framework

**Databases:** SQL Server, PostgreSQL, MySQL, Redis

**Cloud & DevOps:** Azure, Docker, Kubernetes, CI/CD, Azure DevOps, Argo

**AI & ML:** Azure AI Services, Ollama, vLLM, RAG Pipelines, LLM Integration, Claude Code, GitHub Copilot, MCP, Prompt Engineering

**Hardware:** 2× NVIDIA DGX Spark (GB10, 128 GB unified memory each), bridged over ConnectX-7 at 200 Gbps — local inference, fine-tuning, and two-node tensor-parallel serving

---

### 📜 Certifications & Training

| Certification | Issuer | Date |
|---|---|---|
| Azure AI Engineer Associate (AI-102) | Microsoft | Jun 2026 |
| GitHub Copilot (GH-300) | Microsoft | Jun 2026 |
| Azure Fundamentals (AZ-900) | Microsoft | Jun 2026 |
| GitHub Foundations (GH-900) | GitHub | Jun 2026 |
| Azure AI Fundamentals (AI-900) | Microsoft | Apr 2026 |
| Claude Code in Action | Anthropic | Jun 2026 |
| Introduction to Model Context Protocol | Anthropic | Jun 2026 |
| Introduction to Subagents | Anthropic | Jun 2026 |
| Introduction to Agent Skills | Anthropic | Jun 2026 |

📖 **Machine Learning Operations Engineer Associate (AI-300)** — In Progress

---

### 📊 Current Focus

- Studying for the **AI-300** (Microsoft Machine Learning Operations Engineer Associate) — operationalizing ML and generative AI solutions on Azure
- Running local LLM inference and fine-tuning experiments on **DGX Spark** via [SparkBench](https://github.com/vondraysanford/SparkBench)
- Serving **GLM-5.3-Flash** (320B MoE, 4-bit EXL3) tensor-parallel across both Sparks as a local coding model for VS Code — [what that took](https://vondraysanford.com/writing/2026-09-14-320b-on-two-sparks-what-it-actually-takes-to-run-a-mixture-o.html), with [SparkDash](https://github.com/vondraysanford/SparkDash) watching it
- Sharing what I learn at [vondraysanford.com](https://vondraysanford.com) and on [LinkedIn](https://www.linkedin.com/in/vondray-sanford)

---

### 📫 Connect

[![Portfolio](https://img.shields.io/badge/Portfolio-0a0a0b?style=flat&logo=googlechrome&logoColor=white)](https://vondraysanford.com)
[![Hugging Face](https://img.shields.io/badge/Hugging%20Face-FFD21E?style=flat&logo=huggingface&logoColor=black)](https://huggingface.co/vondraysanford)
[![Email](https://img.shields.io/badge/Email-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:vondraysanford@gmail.com)

<!---
vondraysanford/vondraysanford is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
