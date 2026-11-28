### Hi, I'm Arash 👋

**ML Engineer · LLM Agents & Evals · Clinical ML at UCSF · Open-source contributor · Embedded hardware & firmware, PCBs (UC Berkeley) bio-sensing · Bioinformatics (RNA-seq, single-cell)**

Bay Area. Today I build machine learning systems, RAG knowledge bases and LLM agents, and evaluate them carefully enough to trust the numbers. My path runs from bio-sensing hardware and bioinformatics through applied ML in industry to LLM systems.

| Focus | Where | What |
|---|---|---|
| 🤖 **LLM agents & evals** | **Veru365** (fintech) | LLM-as-judge pipelines, red-teaming production financial agents, adversarial evaluation sets, permission-aware retrieval |
| 🏥 **Clinical ML** | **UCSF** | point-in-time clinical trial matching from timestamped notes: a small CPU-trained model that beats 7-8B open-weight LLMs at a fraction of the compute (manuscript in preparation); eye-flow image analysis in Ophthalmology |
| 🔌 **Bio-sensing hardware** | **UC Berkeley**, since 2015 | embedded firmware (C++, Teensy/Arduino), four-layer PCB design, sensor signal processing, computer vision for sensing |
| 📈 **Applied ML in industry** | **Optelligence**, since 2022 | regression and classification models, CNNs and graph neural networks on experimental data, A/B testing |
| 🧬 **Biomedical data** | **National Central University**, Taiwan | blood Raman spectroscopy for cancer detection (manuscript in preparation); bulk and spatial transcriptomics, RNA-seq, single-cell |

Background: BS Bioengineering/Bioinformatics (UC Santa Cruz); Data Science/Analytics (Georgia Tech).

#### Open-source contributions
I fix bugs in the research code behind papers I read: the quiet kind, where a pipeline keeps running but returns plausible, wrong results. Merged so far:

In Stanford MIMI's [Glyph](https://github.com/StanfordMIMI/Glyph/pull/2), which learns sparse concepts from foundation-model embeddings of clinical reports, labs and images, report files were decoded with the machine's locale. On Windows that turned UTF-8 symbols such as ×, ± and ≥ into garbage before tokenization, silently shifting the embeddings. Reports and lab JSON are now read as UTF-8.

In Harvard's [ToolUniverse](https://github.com/mims-harvard/ToolUniverse/pull/911), a library of biomedical tools that LLM agents call, the MedlinePlus genetics-index tool returned 4 rows with empty names (the section URLs) instead of the 2,965 pages in TopicIndex.xml. It now reads the pages one level down, so agents get every gene, condition, chromosome and handbook page.

In [PrismQuant](https://github.com/ForeverBlue816/PrismQuant/pull/6)'s GPTQ quantizer, `fasterquant` called `torch.cuda.synchronize()` unconditionally, so quantizing on a CPU-only machine crashed after the math had finished. It now synchronizes only when the weights are on a GPU.

13+ more fixes are under maintainer review; each is added here once merged.

#### Selected projects
| Project | What it shows |
|---|---|
| [scanpy-claude-agent](https://github.com/arashmparsa/scanpy-claude-agent) | Claude agent + MCP server for single-cell RNA-seq; 95.5% cell-type accuracy on PBMC3k vs 85.7% baseline |
| [latch-rnaseq-de](https://github.com/arashmparsa/latch-rnaseq-de) | Latch workflow for bulk RNA-seq DE (PyDESeq2), validated on planted genes: 97% recall, 95% precision |
| [agent-permission-gateway](https://github.com/arashmparsa/agent-permission-gateway) | Enforcement layer between an LLM agent and its tools: default-deny roles, PII tokenization, hash-chained audit log |
| [pushback-eval](https://github.com/arashmparsa/pushback-eval) | Multi-turn sycophancy eval with a validated grader |
| [insider-cluster-radar](https://github.com/arashmparsa/insider-cluster-radar) | SEC Form 4 pipeline into Postgres and a look-ahead-safe event study (an honest null result) |

#### Certifications
Anthropic Academy — [Building with the Claude API](https://www.anthropic.com/learn) (Nov 2026) · Model Context Protocol: Advanced Topics (Nov 2026) · Claude Code in Action (Nov 2026). CITI Program — Data or Specimens Only Research; Conflicts of Interest (2026).

**Stack:** Python, SQL/PostgreSQL, PyTorch, scikit-learn, XGBoost, Hugging Face, Scanpy/Squidpy, Nextflow, Docker, AWS.

**Elsewhere:** [portfolio](https://arashmparsa.github.io) · [LinkedIn](https://www.linkedin.com/in/arash-p-33166a108)

<sub>Earlier work (2015-2023, incl. DARPA SWARM) lives at github.com/arashmehrabiparsa, an account I can no longer access.</sub>
