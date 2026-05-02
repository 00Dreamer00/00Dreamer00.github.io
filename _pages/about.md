---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

{% if site.google_scholar_stats_use_cdn %}
{% assign gsDataBaseUrl = "https://cdn.jsdelivr.net/gh/" | append: site.repository | append: "@" %}
{% else %}
{% assign gsDataBaseUrl = "https://raw.githubusercontent.com/" | append: site.repository | append: "/" %}
{% endif %}
{% assign url = gsDataBaseUrl | append: "google-scholar-stats/gs_data_shieldsio.json" %}

<span class='anchor' id='about-me'></span>

Hello! I am Ruotao Xu (徐若涛), an M.S. student in Computer Technology at Soochow University (expected 2028). I am based in Suzhou, Jiangsu, China, and I am available for a long-term internship (can start immediately, 5 days/week).

**Contact:** x2503363160@163.com · +86 187-5197-0163  
**Research Interests:** Tool-Integrated Reasoning, Agent, Efficient LLMs, Token Compression, and Domain LLM Evaluation.

# 🔥 News
- *2026.04*: &nbsp;Two paper are accepted by ACL 2026: [ATTC](https://arxiv.org/abs/2604.08281) and [DTSR](https://arxiv.org/abs/2604.06787).

# 📖 Educations
- *2025.09 – 2028.06*, M.S. in Computer Technology, Soochow University (recommended admission).
- *2021.09 – 2025.06*, B.S. in Computer Science and Technology, Zhejiang Sci-Tech University.  
  GPA 3.84/5, rank 3/177; CET-4 581, CET-6 531.

# 🎖 Honors and Awards
- Soochow University Academic Scholarship (**Special Prize**).
- Zhejiang Province **Outstanding Graduate Student**.
- Zhejiang Sci-Tech University **Academic Scholarship**.
- **The Second Prize (National Level)** in the 15th China College Student Service Outsourcing Innovation and Entrepreneurship Competition
- **The Third Prize (National Level)** in the 2024 National English Competition for College Students
- **First Prize (Provincial Level, 1st Place in the Mobile Application Category)** in the 22nd Zhejiang Provincial College Student Multimedia Design Competition
- **Second Prize (Provincial Level)** in the 10th Zhejiang Provincial College Student Service Outsourcing Innovation Application Competition



# 📝 Publications
<!-- - **When to Trust Tools? Adaptive Tool Trust Calibration for Tool-Integrated Math Reasoning**  
  *First Author*, accepted at ACL 2026. Proposed ATTC to calibrate tool trust from generated code confidence; reduced tool neglect and improved performance by 4.1–7.5%.
- **OmniSelect: Adaptive Token Compression Framework for Efficient Omni-modal LLMs**  
  *Co-first Author*, submitted to NeurIPS 2026. Proposed dynamic token compression using AudioCLIP to select guidance signals and adjust pruning ratios; retained 30% tokens with strong performance.
- **When Is Thinking Enough? Early Exit via Sufficiency Assessment for Efficient Reasoning**  
  *Third Author*, accepted at ACL 2026. Proposed DTSR with reasoning-signal detection and sufficiency checks to choose early-exit points; reduced reasoning length by 29–35% without sacrificing performance. -->

**\* denotes equal contribution.**

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ACL 2026</div><img src='images/ATTC.png' width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**When to Trust Tools? Adaptive Tool Trust Calibration for Tool-Integrated Math Reasoning**  

**Ruotao Xu**, Yixin Ji, Yu Luo, Jinpeng Li, Dong Li, Peifeng Li, Juntao Li, Min Zhang

**TL;DR:** We Propose ATTC to calibrate tool trust from generated code confidence; reduced tool neglect and improved performance by 4.1–7.5%.

[![](https://img.shields.io/badge/arXiv-Paper-orange?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.08281)
[![](https://img.shields.io/badge/GitHub-Code-blue?logo=github&logoColor=white)](https://github.com/00Dreamer00/ATTC)
<!-- [![](https://img.shields.io/badge/🤗 HuggingFace-Models-green)](https://huggingface.co/collections/dyyyyyyyy/fapo) -->

</div>
</div>

<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ACL 2026</div><img src='images/DTSR.png' width="100%"></div></div>
<div class='paper-box-text' markdown="1">

**When Is Thinking Enough? Early Exit via Sufficiency Assessment for Efficient Reasoning**  

Yang Xiang, Yixin Ji, **Ruotao Xu**, Dan Qiao, Zheming Yang, Juntao Li, Min Zhang

**TL;DR:** We propose DTSR with reasoning-signal detection and sufficiency checks to choose early-exit points; reduced reasoning length by 29–35% without sacrificing.

[![](https://img.shields.io/badge/arXiv-Paper-orange?logo=arxiv&logoColor=white)](https://arxiv.org/abs/2604.06787)

</div>
</div>



# 🔬 Research & Project Experience

**Nuclear-Device Domain LLM Optimization (CSSC 719 Institute, 2025.04 – 2025.06)**  
*Tech:* Python, data cleaning, LLM-Judge, supervised fine-tuning, instruction tuning, Ray, vLLM, RAG, Milvus  
- Built a domain pretraining corpus (230B tokens) and a general corpus (780B tokens), plus a 6.85M-token high-quality seed dataset.
- Developed a data-quality scoring engine using LLM-Judge + BERT classifier for supervised filtering.
- Synthesized 300k high-quality instruction data and performed full-parameter SFT (Qwen2.5-14B-Instruct, DeepSeek-R1-Distill-Qwen-14B) via LLaMA-Factory, improving nuclear physics benchmark accuracy by 6.9–12.8%.
- Constructed a nuclear-physics benchmark with 12 subfields and 9,844 multiple-choice questions; built distributed auto-evaluation with Ray + vLLM supporting CoT, Rouge-L, and token-level F1.
- Built a domain QA system with RAG, using Milvus vector store and hybrid retrieval (BGE semantic + BM25) with weighted reciprocal-rank fusion.

**Intelligent Contract Processing Agent (Suzhou Bank, 2025.01 – 2025.03)**  
*Tech:* Python, OCR, LangChain, LangGraph, RAG, ChromaDB  
- Cleaned open-source datasets and contract documents to build 40k instruction-tuning samples (contract classification, entity extraction, etc.).
- Built a legal benchmark from national judicial exam questions and legal consultation docs (2,500 multiple-choice and 300 subjective questions).
- LoRA-tuned Qwen2.5-7B-Instruct, outperforming the base and open-source legal models on the test set.
- Implemented modules for contract classification, clause extraction, contract review, and legal QA; added RAG-based risk identification.
- Built a LangGraph agent with a loop of analysis → evidence review → drafting → review → revise, using a state machine to preserve context and consistency.
