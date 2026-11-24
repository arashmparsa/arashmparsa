### Hi, I'm Arash 👋

Data scientist / ML engineer in the Bay Area. I build models and LLM systems that hold up under careful evaluation.

- **Clinical ML** with Dr. Vivek Rudrapatna's group at UCSF: point-in-time clinical trial matching from timestamped notes, a small CPU-trained head that beats 7-8B open-weight LLMs at a fraction of the compute (manuscript in preparation).
- **LLM agents, RAG and evaluation** at Veru365 (fintech): red-teaming production financial agents, LLM-as-judge pipelines, permission-aware retrieval.
- **Bioinformatics and biophotonics**: bulk and spatial transcriptomics, blood Raman spectroscopy for cancer detection (ongoing collaboration, not yet published).

Background: BS Bioengineering/Bioinformatics (UC Santa Cruz), MS Data Science/Analytics (Georgia Tech).

#### Open-source contributions
- [StanfordMIMI/Glyph#2](https://github.com/StanfordMIMI/Glyph/pull/2) (merged): reads clinical reports as UTF-8 so non-ASCII text is not silently garbled before embedding
- [gersteinlab/MedicalAgentsBench#10](https://github.com/gersteinlab/MedicalAgentsBench/pull/10): fixes 79 MedExQA answer keys stored one row out of place, with a reproducible audit script
- [phai-lab/behavior-uncloning#1](https://github.com/phai-lab/behavior-uncloning/pull/1): validation loss weighted by sample count, so a short last batch no longer skews it
- [cyber-arena-ai/octagon#4](https://github.com/cyber-arena-ai/octagon/pull/4): CyberArena tokens-per-second metric no longer inflated by overlapping model calls
- [ESPARGOS/pyespargos#17](https://github.com/ESPARGOS/pyespargos/pull/17): helper for mapping Wi-Fi CSI onto an IFFT grid (from the HT40 subcarrier-mapping analysis in [#9](https://github.com/ESPARGOS/pyespargos/issues/9))
- Also: [CORAL#2](https://github.com/zou-group/CORAL/pull/2), [PhysioWave#4](https://github.com/ForeverBlue816/PhysioWave/pull/4), [PrismQuant#6](https://github.com/ForeverBlue816/PrismQuant/pull/6), [PCBRouteAgent#5](https://github.com/chip-ai-agent/PCBRouteAgent/pull/5)

#### Selected projects
| Project | What it shows |
|---|---|
| [scanpy-claude-agent](https://github.com/arashmparsa/scanpy-claude-agent) | Claude agent + MCP server for single-cell RNA-seq; 95.5% cell-type accuracy on PBMC3k vs 85.7% baseline |
| [latch-rnaseq-de](https://github.com/arashmparsa/latch-rnaseq-de) | Latch workflow for bulk RNA-seq DE (PyDESeq2), validated on planted genes: 97% recall, 95% precision |
| [agent-permission-gateway](https://github.com/arashmparsa/agent-permission-gateway) | Enforcement layer between an LLM agent and its tools: default-deny roles, PII tokenization, hash-chained audit log |
| [pushback-eval](https://github.com/arashmparsa/pushback-eval) | Multi-turn sycophancy eval with a validated grader |
| [insider-cluster-radar](https://github.com/arashmparsa/insider-cluster-radar) | SEC Form 4 pipeline into Postgres and a look-ahead-safe event study (an honest null result) |

**Stack:** Python, SQL/PostgreSQL, PyTorch, scikit-learn, XGBoost, Hugging Face, Scanpy/Squidpy, Nextflow, Docker, AWS.

**Elsewhere:** [portfolio](https://arashmparsa.github.io) · [LinkedIn](https://www.linkedin.com/in/arash-p-33166a108)

<sub>Earlier work (2015-2023, incl. DARPA SWARM) lives at github.com/arashmehrabiparsa, an account I can no longer access.</sub>
