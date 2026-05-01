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

Hello! I am Ruotao Xu (徐若涛), an M.S. student in Computer Technology at Soochow University (expected 2028). I am based in Nanjing, Jiangsu, China, and I am available for a long-term internship (can start immediately, 5 days/week).

**Contact:** x2503363160@163.com · +86 187-5197-0163  
**Google Scholar:** [https://scholar.google.com/citations?hl=en&user=uw3bKYIAAAAJ](https://scholar.google.com/citations?hl=en&user=uw3bKYIAAAAJ&view_op=list_works&gmla=AIqSsVtpRSzI2qaXy6ek77P-5yH8AL2ePwajUzQEqQ5NSS-N04Qw5h3NaIiJCVAYR-rWq8PMpwizgMkXwANEERuz)

**Research Interests:** tool-integrated reasoning, efficient LLMs, token compression, RAG, and domain LLM evaluation.

# 📝 Publications
<div class="paper-box">
  <div class="paper-box-image">
    <div class="badge">ACL 2026</div>
    <img src="{{ '/images/publications/attc.png' | relative_url }}" alt="ATTC teaser">
  </div>
  <div class="paper-box-text">
    <h3>When to Trust Tools? Adaptive Tool Trust Calibration for Tool-Integrated Math Reasoning</h3>
    <p class="paper-box-authors">First Author · Accepted at ACL 2026</p>
    <p><strong>TL;DR:</strong> Proposed ATTC to calibrate tool trust from generated code confidence; reduced tool neglect and improved performance by 4.1–7.5%.</p>
    <div class="paper-box-links">
      <span class="paper-tag paper-tag--arxiv"><i class="ai ai-arxiv" aria-hidden="true"></i> arXiv</span>
      <span class="paper-tag paper-tag--paper"><i class="fas fa-file-alt" aria-hidden="true"></i> Paper</span>
      <span class="paper-tag paper-tag--github"><i class="fab fa-github" aria-hidden="true"></i> GitHub</span>
      <span class="paper-tag paper-tag--code"><i class="fas fa-code" aria-hidden="true"></i> Code</span>
      <span class="paper-tag paper-tag--models"><i class="fas fa-robot" aria-hidden="true"></i> Models</span>
    </div>
  </div>
</div>

<div class="paper-box">
  <div class="paper-box-image">
    <div class="badge">NeurIPS 2026</div>
    <img src="{{ '/images/publications/omniselect.png' | relative_url }}" alt="OmniSelect teaser">
  </div>
  <div class="paper-box-text">
    <h3>OmniSelect: Adaptive Token Compression Framework for Efficient Omni-modal LLMs</h3>
    <p class="paper-box-authors">Co-first Author · Submitted to NeurIPS 2026</p>
    <p><strong>TL;DR:</strong> Proposed dynamic token compression using AudioCLIP to select guidance signals and adjust pruning ratios; retained 30% tokens with strong performance.</p>
    <div class="paper-box-links">
      <span class="paper-tag paper-tag--arxiv"><i class="ai ai-arxiv" aria-hidden="true"></i> arXiv</span>
      <span class="paper-tag paper-tag--paper"><i class="fas fa-file-alt" aria-hidden="true"></i> Paper</span>
      <span class="paper-tag paper-tag--github"><i class="fab fa-github" aria-hidden="true"></i> GitHub</span>
      <span class="paper-tag paper-tag--code"><i class="fas fa-code" aria-hidden="true"></i> Code</span>
      <span class="paper-tag paper-tag--models"><i class="fas fa-robot" aria-hidden="true"></i> Models</span>
    </div>
  </div>
</div>

<div class="paper-box">
  <div class="paper-box-image">
    <div class="badge">ACL 2026</div>
    <img src="{{ '/images/publications/dtsr.png' | relative_url }}" alt="DTSR teaser">
  </div>
  <div class="paper-box-text">
    <h3>When Is Thinking Enough? Early Exit via Sufficiency Assessment for Efficient Reasoning</h3>
    <p class="paper-box-authors">Third Author · Accepted at ACL 2026</p>
    <p><strong>TL;DR:</strong> Proposed DTSR with reasoning-signal detection and sufficiency checks to choose early-exit points; reduced reasoning length by 29–35% without sacrificing performance.</p>
    <div class="paper-box-links">
      <span class="paper-tag paper-tag--arxiv"><i class="ai ai-arxiv" aria-hidden="true"></i> arXiv</span>
      <span class="paper-tag paper-tag--paper"><i class="fas fa-file-alt" aria-hidden="true"></i> Paper</span>
      <span class="paper-tag paper-tag--github"><i class="fab fa-github" aria-hidden="true"></i> GitHub</span>
      <span class="paper-tag paper-tag--code"><i class="fas fa-code" aria-hidden="true"></i> Code</span>
      <span class="paper-tag paper-tag--models"><i class="fas fa-robot" aria-hidden="true"></i> Models</span>
    </div>
  </div>
</div>

# 🎖 Honors and Awards
- Zhejiang Province Outstanding Graduate.
- Soochow University Academic Scholarship (Special Prize).

# 📖 Education
- *2025.09 – 2028.06*, M.S. in Computer Technology, Soochow University (recommended admission).
- *2021.09 – 2025.06*, B.S. in Computer Science and Technology, Zhejiang University of Technology.  
  GPA 3.84/5, rank 3/177; CET-4 581, CET-6 531.

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
