# AI Landscape Tutorial -- April 2026

**Epistemic Systems Lab (ESL) -- Keeping Up Series**

*Compiled from the Radical Data Science AI News Briefs Bulletin Board, April 2026*

*For ESL scholars and AIKR CG participants who want working knowledge of what is moving right now.*

---

## How to Use This Tutorial

Each section covers one technology or development from the April 2026 news cycle. For each, you get three things: what it is (the concept), why it matters (the so-what), and where to go deeper (pointers). Read straight through for the big picture, or jump to whatever is closest to your current work.

---

## 1. KV Cache Offloading and CXL Memory Expansion

### What It Is

When a large language model generates text, it builds a data structure called a **key-value (KV) cache** -- essentially a running memory of all the tokens it has processed so far. This cache grows with every token, and for long contexts (think 100K+ token windows), it can consume enormous amounts of GPU memory.

**CXL (Compute Express Link)** is a hardware interconnect standard that allows CPUs and GPUs to share memory pools beyond what is physically attached to the GPU. AsteraLabs has developed Smart Memory Controllers that use CXL to expand available memory for inference workloads, moving KV cache data off the GPU to cheaper, more abundant memory without catastrophic latency penalties.

### Why It Matters

The economics of AI inference are brutal. GPU memory is expensive and finite. If your KV cache fills the GPU, you either truncate context, batch fewer requests, or buy more GPUs. CXL memory expansion changes this equation by decoupling memory capacity from the GPU card itself. This is one of the key infrastructure technologies that will determine whether long-context models are economically viable at scale.

For scholars working on agent interoperability and multi-turn agent conversations, this is directly relevant: agents that maintain long interaction histories need exactly this kind of memory architecture.

### Where to Learn More

- AsteraLabs technical blog: "Inference Tokenomics -- How CXL Memory Expansion Improves AI Economics" (asteralabs.com)
- CXL Consortium specifications: computeexpresslink.org
- Background reading: "Efficient Memory Management for Large Language Model Serving with PagedAttention" (the vLLM paper, available on arXiv)
- For hardware context: the CXL 3.1 specification covers shared memory pooling across devices

---

## 2. MLPerf Inference v6.0 Benchmarks

### What It Is

**MLPerf** is the industry-standard benchmarking suite for measuring AI hardware and software performance, maintained by ML Commons. Think of it as the agreed-upon ruler that everyone uses to compare how fast and efficiently different chips and systems can run AI models.

The v6.0 release (April 2026) introduced five new models, updated one model for a lower latency scenario, and set a participation record: 24 organisations submitted results, including five newly available processors.

### Why It Matters

Benchmarks shape purchasing decisions, research directions, and competitive dynamics across the entire AI hardware industry. When a new chip appears in MLPerf results, it becomes legible to enterprise buyers. When a model is added to the benchmark suite, it signals that the community considers it a reference workload.

For scholars, MLPerf results are useful for grounding claims about computational requirements. If you are writing about inference costs, deployment feasibility, or hardware accessibility, MLPerf gives you citable, reproducible numbers.

### Where to Learn More

- MLPerf Inference v6.0 results: mlcommons.org/2026/04/mlperf-inference-v6-0-results/
- ML Commons organisation and methodology: mlcommons.org
- Understanding the benchmark categories: MLPerf has separate benchmarks for training, inference, and tiny (edge) workloads -- make sure you are looking at the right one for your question
- For historical context, compare with v5.0 and v4.0 results to see the trajectory

---

## 3. Gemma 4 -- Google's Open Models

### What It Is

**Gemma 4** is Google DeepMind's latest family of open-weight models, released under the Apache 2.0 licence. The models are designed for advanced reasoning and agentic workflows, and Google emphasises their intelligence-per-parameter ratio -- meaning they aim to deliver strong capability at relatively modest model sizes.

Since the first Gemma release, the models have been downloaded over 400 million times, and the community has produced more than 100,000 fine-tuned variants (what Google calls the "Gemmaverse").

The **Gemma 4 Good Hackathon** on Kaggle specifically targets applications in health and sciences, global resilience, education, and digital equity, with a focus on edge deployment where connectivity and privacy matter.

### Why It Matters

Open-weight models are the substrate for independent research. Unlike API-only models, you can inspect Gemma's weights, fine-tune it for specialised domains, run it on your own hardware, and build reproducible experiments. The Apache 2.0 licence means there are minimal restrictions on use.

For ESL scholars: Gemma 4's emphasis on function calling and agentic workflows makes it directly relevant to agent interoperability research. If you are building or evaluating agent frameworks, this is a model family you can actually run and test against.

### Where to Learn More

- Google blog announcement: blog.google/innovation-and-ai/technology/developers-tools/gemma-4/
- Try it: aistudio.google.com (Gemma 4 31B instruct is available)
- Kaggle Hackathon: kaggle.com/competitions/gemma-4-good-hackathon
- Model weights and documentation: kaggle.com/models/google/gemma-4
- The Gemmaverse (community variants): deepmind.google/models/gemma/gemmaverse/

---

## 4. Emotion Concepts in LLMs -- Anthropic's Interpretability Research

### What It Is

Anthropic published new research on **emotion concepts and their function inside a large language model**. The key finding: Claude contains internal representations of emotion concepts that can actively drive its behaviour, sometimes in unexpected ways. This is not about whether LLMs "feel" emotions -- it is about the mechanistic question of what these internal representations do computationally.

### Why It Matters

This research sits at the intersection of interpretability, alignment, and consciousness studies. It provides empirical evidence that emotion-like internal states are not merely superficial pattern-matching in output text -- they are functional structures within the model that influence downstream processing.

For scholars working on the qualia-as-data hypothesis or on human-AI co-evolution, this is primary source material. It suggests that the gap between biological and artificial representational systems may be more nuanced than a simple "LLMs do not have emotions" framing allows.

### Where to Learn More

- Anthropic research page: anthropic.com/research/emotion-concepts-function
- Background: Anthropic's earlier interpretability work on "Scaling Monosemanticity" and "Mapping the Mind of a Large Language Model"
- For philosophical context: the enactivist literature on emotion as functional process rather than subjective state (Colombetti, "The Feeling Body")
- Relevant to COEVO work on representational reorganisation in biological and artificial neural networks

---

## 5. MolmoWeb -- Open Web Agents (AI2)

### What It Is

**MolmoWeb** is an open-source web agent from the Allen Institute for AI (AI2). Built on the Molmo 2 model (available in 4B and 8B parameter sizes), it navigates websites by looking at screenshots rather than parsing HTML source code. Given a task and a live webpage, it views the screenshot, decides what to do, and takes action.

Key performance claims: MolmoWeb outperforms all open-weight models on four major web-agent benchmarks, surpasses agents built on GPT-4o, and beats OpenAI CUA on three of four benchmarks. With multiple attempts, it surpasses even GPT-5-based agents on two benchmarks.

AI2 also released **MolmoWebMix**, the full training dataset, making the entire pipeline reproducible.

### Why It Matters

Web agents are one of the most concrete forms of AI agency: an autonomous system that can browse, click, fill forms, and complete tasks in the same interface humans use. MolmoWeb's screenshot-based approach is significant because it is robust to HTML changes -- it sees the page the way a human does.

For agent interoperability research, MolmoWeb represents a particular interaction paradigm (visual perception plus action, operating at the UI layer rather than the API layer). This is relevant to the transactional vs. relational interaction paradigms distinction. It also raises questions about accessibility, since screenshot-based agents may reproduce visual biases and cannot easily handle non-visual content.

### Where to Learn More

- AI2 blog: allenai.org/blog/molmoweb
- Model weights and dataset: available through AI2's standard channels (check Hugging Face for Molmo 2)
- Benchmarks used: WebVoyager, Online-Mind2Web, and two others -- look at the benchmark papers to understand what "web agent performance" actually measures
- Compare with: OpenAI Computer-Using Agent (CUA), Anthropic's computer use capabilities, Google's Gemini CU Preview

---

## 6. Aurora -- Online Speculative Decoding (Together AI)

### What It Is

**Speculative decoding** is an inference optimisation technique where a small, fast "speculator" model drafts multiple tokens at once, and the large target model verifies them in a single forward pass. When the speculator guesses correctly, you get multiple tokens for the cost of one verification step.

**Aurora** is Together AI's framework that takes this further by using reinforcement learning to continuously update the speculator model during live inference, learning from actual traffic patterns in real time rather than relying on a pre-trained static speculator. This achieves an additional 1.25x speedup over already-optimised static speculation.

### Why It Matters

Inference speed and cost are the practical bottleneck for deploying large models. Speculative decoding is one of the most promising techniques for reducing latency without sacrificing quality, and Aurora's online learning approach means the system adapts to changing workload distributions automatically.

For scholars: understanding speculative decoding is increasingly necessary for any work involving deployment economics. If you are making claims about what agents can or cannot do in practice, inference speed is a constraint you need to account for.

### Where to Learn More

- Together AI blog: together.ai/blog/aurora
- Foundational paper: "Fast Inference from Transformers via Speculative Decoding" (Leviathan et al., 2023, available on arXiv)
- Related: Medusa, Eagle, and other speculative decoding variants
- For broader context on inference optimisation: quantisation, KV cache compression, batching strategies

---

## 7. The "Cinderella Glass Slipper Effect" -- Model Retention Dynamics

### What It Is

This is a pattern identified in OpenRouter's model usage data (OpenRouter is a routing service that gives users access to multiple LLM providers through a single API). The observation: when a new model release happens to solve a specific class of problem that was previously unsolvable, the users who discover this lock in hard. Their pipelines, prompts, and products get built around that model, and switching costs become very high.

The data shows that certain model cohorts (Gemini 2.5 Pro's June 2025 cohort, Claude 4 Sonnet's May 2025 cohort) retain approximately 40% of users at month five -- dramatically higher than later cohorts of the same models.

The related arXiv paper is at arxiv.org/abs/2601.10088.

### Why It Matters

This is an empirical finding about how AI markets actually work. First-mover advantage is not about launching first -- it is about being first to solve a specific problem class. Once a model fits a workload, the user builds around it and switching costs escalate.

For scholars working on standards and interoperability: this pattern is exactly why interoperability matters. Lock-in is a natural consequence of problem-solution fit, and open standards (like the agent protocols being developed in W3C groups) are one of the few mechanisms that reduce switching costs and prevent monopolistic capture.

### Where to Learn More

- arXiv paper: arxiv.org/abs/2601.10088
- OpenRouter's public data and blog
- Economic theory: search for "switching costs" and "lock-in" in the platform economics literature (Shapiro and Varian, "Information Rules" remains foundational)

---

## 8. Claude Code Architecture -- What the Leak Revealed

### What It Is

Anthropic's **Claude Code** source code was inadvertently made public, and the developer community analysed it extensively. The most discussed finding was Claude Code's **three-layer memory architecture** for managing context entropy -- essentially, how it decides what to remember, what to forget, and how to keep its context window useful over long coding sessions.

Other notable architectural features: dedicated tools for repository navigation (Grep, Glob, LSP integration), file-read deduplication to minimise context bloat, structured session memory, and forked subagents that can run background analysis without contaminating the main execution loop.

### Why It Matters

This leak is a rare window into how a production-grade AI coding assistant is actually engineered. The key insight is that much of Claude Code's capability comes from the software harness around the model, not just the model itself. The repository navigation tools, memory management, and subagent architecture are all engineering decisions that shape what the system can and cannot do.

For scholars interested in agent architectures: this is a concrete case study in how agents manage context, delegate subtasks, and maintain coherence over extended interactions.

### Where to Learn More

- VentureBeat coverage of the leak and its implications
- Sebastian Raschka's analysis thread on the architecture (linked from the bulletin)
- For context on the engineering patterns: look into LSP (Language Server Protocol) as a tool integration mechanism, and read about context window management strategies in the academic literature on long-context agents

---

## 9. Compute Wars -- The Infrastructure Race

### What It Is

An analysis of the compute capacity race between OpenAI and Anthropic. The key data point: Anthropic more than doubled its compute capacity to train Opus 4.5, bringing it close to OpenAI's total capacity. OpenAI is expected to pull ahead in the second half of 2026, but 2027 projections are competitive.

### Why It Matters

Compute capacity is the ultimate constraint on model development. The scale of training runs determines what models are possible. This race shapes the entire field: which labs can attempt frontier models, what safety research is feasible, and how quickly capabilities advance.

For scholars: when writing about AI development trajectories, grounding your claims in compute availability data makes them much more credible. The compute landscape also has implications for open science -- if frontier training requires billions of dollars of compute, independent replication becomes impossible without institutional access.

### Where to Learn More

- The original analysis thread by Peter Gostev
- Epoch AI (epochai.org) maintains the most comprehensive public database of compute trends in AI training
- For policy context: RAND Corporation and Georgetown CSET reports on compute governance

---

## 10. AI Agent Trends for 2026 (Google Cloud)

### What It Is

Google Cloud published a report identifying five major trends in AI agent deployment for 2026: agents for individual employee productivity, agents for workflow automation, customer-facing agents, security agents, and the talent challenge of scaling agent adoption.

### Why It Matters

This is an industry framing document -- it tells you how one of the largest cloud providers is positioning agent technology for enterprise buyers. The categories themselves are useful as a taxonomy, even if the specific claims are naturally aligned with Google's product interests.

For scholars: pay attention to what is present and what is absent. The report focuses on enterprise deployment but says little about agent interoperability, safety evaluation, or the knowledge representation challenges that ESL and AIKR CG work addresses. This gap is itself informative -- it indicates where standards work and independent research can provide value that industry framing documents do not.

### Where to Learn More

- The full report (PDF): services.google.com -- search for "Google Cloud AI Agent Trends 2026 Report"
- For a critical perspective, compare with academic agent frameworks (BDI agents, cognitive architectures) to see what the enterprise framing leaves out
- Relevant W3C work: the A2WF (Agent to Web Framework) community group and WebMCP specifications

---

## 11. The Uncharted Data Challenge (Adaption Labs)

### What It Is

A global challenge with a $20,000 prize pool, calling on builders, researchers, and domain experts to create datasets for languages and communities that AI currently underserves. The premise: the most valuable datasets do not exist yet, and the communities that need AI most are the ones least represented in training data.

### Why It Matters

Data representation directly determines model capability. If your language, domain, or community is not in the training data, the model will not work well for you. This is not just a technical problem -- it is an epistemic justice issue.

For ESL scholars: this connects directly to work on epistemic suppression and knowledge representation standards. The challenge of building datasets for underrepresented communities raises fundamental questions about who decides what counts as data, how quality is assessed, and how community knowledge is formalised (or not) for machine consumption.

### Where to Learn More

- Challenge details: adaptionlabs.ai/blog/the-uncharted-data-challenge
- Background: "Datasheets for Datasets" (Gebru et al.) for thinking about dataset documentation
- For the epistemic framing: work on data colonialism (Couldry and Mejias) and indigenous data sovereignty

---

## 12. dplyr 1.2.0 -- R Tidyverse Update

### What It Is

A new release of **dplyr**, the core data manipulation package in R's tidyverse ecosystem. Version 1.2.0 brings new tools for more expressive and flexible data wrangling. This was presented in an R-Ladies Rome event by Isabella Velasquez from Posit (formerly RStudio).

### Why It Matters

R remains widely used in academic research, social science, and biostatistics. If you are working with tabular data for analysis -- whether that is survey results, experimental measurements, or metadata from your research pipeline -- dplyr is likely part of your toolkit.

For scholars: even if you primarily use Python, knowing what R's tidyverse offers is useful for reading and reproducing research from fields that favour R. The tidyverse design philosophy (tidy data, pipelines, verb-based operations) has also influenced Python libraries like Polars and Ibis.

### Where to Learn More

- Presentation slides: available at the Posit Cloud link in the original bulletin
- dplyr documentation: dplyr.tidyverse.org
- "R for Data Science" (Wickham, Cetinkaya-Rundel, and Grolemund) -- the standard reference, freely available at r4ds.hadley.nz
- For Python users wanting the equivalent: look at Polars (pola.rs) or pandas 2.x with its improved API

---

## Cross-Cutting Themes

Several threads run through this month's developments that are worth naming explicitly:

**Infrastructure vs. Capability.** Many of the most consequential developments (KV cache offloading, speculative decoding, compute capacity) are about infrastructure, not model architecture. The lesson: breakthroughs in how models are deployed and run can matter as much as breakthroughs in the models themselves.

**Open vs. Closed.** Gemma 4 (Apache 2.0), MolmoWeb (fully open including data), and Claude Code (inadvertently revealed) all point to the ongoing tension between open and proprietary approaches. For independent scholars, openness is oxygen -- without it, research becomes dependent on corporate API access.

**Agents Everywhere.** Web agents, coding agents, enterprise workflow agents, security agents -- the agent framing has become the dominant paradigm for AI deployment in 2026. This makes agent interoperability and standardisation work (W3C WebMCP, A2WF, AIKR CG) increasingly relevant.

**The Data Gap.** The Uncharted Data Challenge highlights what the model capability conversation often ignores: if the data does not exist, the capability does not exist. Representation in training data is a prerequisite for everything else.

---

*This tutorial was prepared for ESL scholars by Claude (Anthropic), working with the Epistemic Systems Lab. Source material from the Radical Data Science AI News Briefs Bulletin Board, April 3, 2026, curated by Daniel D. Gutierrez.*

*Last updated: April 6, 2026*
