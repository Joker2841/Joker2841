<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0D1117,100:1B2735&height=200&section=header&text=Sai%20Girish%20Anga&fontSize=60&fontColor=58A6FF&fontAlignY=38&desc=Software%20Engineer%20-%20Backend%2C%20Systems%2C%20Applied%20AI&descSize=18&descAlignY=58&animation=fadeIn" alt="header banner"/>
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com/?font=Fira+Code&size=20&pause=1500&color=58A6FF&center=true&vCenter=true&width=650&lines=Backend+%26+Systems+Engineer;Building+AI+Evaluation+Infrastructure;Codeforces+Expert+-+Max+Rating+1803;Open+to+Full-Time+SDE+Roles" alt="Typing SVG"/>
</p>

<p align="center">
  <a href="https://tensen.dev"><img src="https://img.shields.io/badge/Blog-tensen.dev-0D1117?style=for-the-badge&logo=hashnode&logoColor=58A6FF&labelColor=0D1117" alt="Blog"/></a>
  <a href="https://www.linkedin.com/in/sai-girish-anga"><img src="https://img.shields.io/badge/LinkedIn-0D1117?style=for-the-badge&logo=linkedin&logoColor=58A6FF&labelColor=0D1117" alt="LinkedIn"/></a>
  <a href="https://codeforces.com/profile/Varun301004"><img src="https://img.shields.io/badge/Codeforces-Expert%201803-0D1117?style=for-the-badge&logo=codeforces&logoColor=58A6FF&labelColor=0D1117" alt="Codeforces"/></a>
  <a href="mailto:jokerbj2841@gmail.com"><img src="https://img.shields.io/badge/Email-0D1117?style=for-the-badge&logo=gmail&logoColor=58A6FF&labelColor=0D1117" alt="Email"/></a>
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=Joker2841&style=flat-square&color=58A6FF&label=Profile+Views" alt="Profile Views"/>
</p>

<p align="center">Open to full-time SDE, backend, and infrastructure roles. Based in India. Available immediately.</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=0:0D1117,100:58A6FF&height=3&section=header" alt="divider"/>
</p>

<h3 align="center">Impact at a glance</h3>

<p align="center">
  <img src="https://img.shields.io/badge/Sastran-28x%20Faster%20Lookups-58A6FF?style=for-the-badge&labelColor=0D1117" alt="Sastran speedup"/>
  <img src="https://img.shields.io/badge/Sastran-96.2%25%20Recall%20at%204x%20Compression-58A6FF?style=for-the-badge&labelColor=0D1117" alt="Sastran quantization"/>
  <img src="https://img.shields.io/badge/Coherence-100%25%20Precision%20and%20Recall-58A6FF?style=for-the-badge&labelColor=0D1117" alt="Coherence accuracy"/>
</p>
<p align="center">
  <img src="https://img.shields.io/badge/LLM%20Router-41%25%20Cost%20Reduction-58A6FF?style=for-the-badge&labelColor=0D1117" alt="LLM router savings"/>
  <img src="https://img.shields.io/badge/Redrob-0.929%20NDCG%20at%20100K%20Scale-58A6FF?style=for-the-badge&labelColor=0D1117" alt="Redrob NDCG"/>
  <img src="https://img.shields.io/badge/Sarcasm%20Model-94.77%25%20Macro%20F1-58A6FF?style=for-the-badge&labelColor=0D1117" alt="Sarcasm model F1"/>
</p>

<br/>

## About me

I graduated in 2026 with a CS degree from IIT Guwahati. Most of what I build sits underneath the parts of software people actually see: storage engines, retrieval pipelines, the plumbing that decides whether a system holds up under load or just falls over quietly.

I like problems where correctness is checkable and performance is measurable. That is probably why competitive programming stuck with me longer than most hobbies do.

## Right now

- Interviewing for full-time SDE, backend, and infrastructure roles
- Writing occasionally at tensen.dev
- Climbing toward Candidate Master on Codeforces

<br/>

## Featured projects

<table>
<tr>
<td width="50%" valign="top">

### Sastran
**Unified key-value and vector storage engine**
Rust, LSM-tree, HNSW, WAL, Criterion

A crash-safe storage engine that puts an LSM-tree and an HNSW vector index behind one durability story, so an exact key lookup and a similarity search can hit the same data without running two separate systems kept in sync by hand. Bloom filters cut absent-key lookups from 2.63 microseconds to 94 nanoseconds, about 28x faster. Vector deletes repair their neighbors properly instead of leaving tombstones, so recall stays above 0.80 after removing 30% of a 2,000-vector index. About 190 tests, zero unsafe code.

[github.com/Joker2841/sastran](https://github.com/Joker2841/sastran)

</td>
<td width="50%" valign="top">

### Coherence
**A consistency layer for AI memory**
Python, Cognee, Kuzu, LanceDB

Built for the WeMakeDevs and Cognee hackathon. Cognee gives an agent perfect recall; Coherence makes sure that recall never quietly holds two contradictory facts at once. Contradictions get caught with deterministic rules first, and an LLM only steps in for the genuinely ambiguous cases, after a vector gate narrows the field from 11 candidates down to 1. 15 tests passing, 100% precision and recall across 36 labeled judgments, and a guardrail that got all 16 of 16 agent-action calls right in testing.

[github.com/Joker2841/coherence](https://github.com/Joker2841/coherence)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### Tokenless
**A local-first routing agent**
Python, LoRA, GGUF, Docker

Built for the AMD Developer Hackathon. A 1.5B parameter model, fine-tuned with LoRA on a dataset generated for the task, answers what it can locally. Deterministic checks back it up instead of trusting it outright: a Python interpreter for math, a sandbox for generated code, spaCy for named entities. Runs inside 4 GB of RAM and two vCPUs with no GPU, spends zero hosted-model tokens, and hit 100% on the evaluation benchmarks.

[github.com/Joker2841/router-agent](https://github.com/Joker2841/router-agent)

</td>
<td width="50%" valign="top">

### RAG-aware multi-tier LLM routing
**B.Tech thesis**
Python, XGBoost, FAISS

A router that sends each query to the cheapest model that can still answer it correctly, based on how good the retrieved passage looks and how hard the question actually is. Tested across three datasets and 1,500 queries against a 10.5 million passage Wikipedia index. Cuts inference cost by about 41% while preserving 93.3% of answer quality.

[github.com/Joker2841/rag-aware-routing](https://github.com/Joker2841/rag-aware-routing)

</td>
</tr>
</table>

### Redrob - candidate ranking without reading the prose
Python, Ollama, NDCG evaluation

A ranking engine built after noticing the underlying dataset's resume text was templated and mostly meaningless, repeated almost word for word across unrelated candidates. Ranks 100,000 synthetic candidates down to a defensible top 100 using structural signals instead: title, company, years of experience, availability. Runs on a single CPU in under five minutes and scores 0.929 NDCG at 10.

[huggingface.co/spaces/sai001122/redrob-ranker-demo](https://huggingface.co/spaces/sai001122/redrob-ranker-demo)

## More work

- **DocuMind** - a RAG document assistant with FastAPI, React, and FAISS, built to actually run rather than just demo well. [repo](https://github.com/Joker2841/document-qa-rag-new)
- **Runway** - an agent that does the first real step of a task instead of just reminding you about it, built on Gemini through Google AI Studio. [repo](https://github.com/Joker2841/Runway)
- **Sarcasm detection** - a fine-tuned DeBERTa-v3 model with a custom affective-feature fusion layer, reaching 94.77% macro-F1, about 2.56 points above the published COLING 2020 benchmark.
- **NIDS** - a real-time network intrusion detector in Python, processing 1,000 to 3,000 packets per second. The project where I met Python's GIL bottleneck in person. [repo](https://github.com/Joker2841/NIDS)
- Codeforces archive, and a Bengaluru Traffic Police x Flipkart traffic demand hackathon (Gridlock 2.0).

<br/>

## How I work

A few things I have actually learned from building these, not borrowed from somewhere else.

**Measure before optimizing.** The 28x bloom filter speedup in Sastran came from writing the benchmark before writing the optimization. The 41% routing cost reduction came from labeling 1,500 queries with GPU oracle data before training anything. In Redrob, I dropped several signals that felt obviously useful, like keyword density and duplicate description detection, down to zero weight once I measured that they added no ranking value across the full 100,000 candidate pool.

**Learn by building.** Rust at any real depth came from building Sastran, not from a course. HNSW came from reading the Malkov-Yashunin paper and implementing it, not from wrapping someone else's library.

**Comfortable being wrong.** Competitive programming means my code gets judged against test cases every weekend, in public. Disagreement and error read as information, not as a threat.

**Honest about scope.** Sastran is a single-node engine, not a distributed system. DocuMind is production-style, not battle-tested in actual production. I would rather finish something small well than gesture at something bigger I have not actually built.

<br/>

## Tech stack

<p align="center">
  <img src="https://img.shields.io/badge/Rust-0D1117?style=for-the-badge&logo=rust&logoColor=58A6FF" alt="Rust"/>
  <img src="https://img.shields.io/badge/C++-0D1117?style=for-the-badge&logo=cplusplus&logoColor=58A6FF" alt="C++"/>
  <img src="https://img.shields.io/badge/Python-0D1117?style=for-the-badge&logo=python&logoColor=58A6FF" alt="Python"/>
  <img src="https://img.shields.io/badge/Java-0D1117?style=for-the-badge&logo=openjdk&logoColor=58A6FF" alt="Java"/>
  <img src="https://img.shields.io/badge/SQL-0D1117?style=for-the-badge&logo=postgresql&logoColor=58A6FF" alt="SQL"/>
</p>
<p align="center">
  <img src="https://img.shields.io/badge/FastAPI-0D1117?style=for-the-badge&logo=fastapi&logoColor=58A6FF" alt="FastAPI"/>
  <img src="https://img.shields.io/badge/Node.js-0D1117?style=for-the-badge&logo=nodedotjs&logoColor=58A6FF" alt="Node.js"/>
  <img src="https://img.shields.io/badge/PostgreSQL-0D1117?style=for-the-badge&logo=postgresql&logoColor=58A6FF" alt="PostgreSQL"/>
  <img src="https://img.shields.io/badge/MongoDB-0D1117?style=for-the-badge&logo=mongodb&logoColor=58A6FF" alt="MongoDB"/>
  <img src="https://img.shields.io/badge/Redis-0D1117?style=for-the-badge&logo=redis&logoColor=58A6FF" alt="Redis"/>
</p>
<p align="center">
  <img src="https://img.shields.io/badge/PyTorch-0D1117?style=for-the-badge&logo=pytorch&logoColor=58A6FF" alt="PyTorch"/>
  <img src="https://img.shields.io/badge/HuggingFace-0D1117?style=for-the-badge&logo=huggingface&logoColor=58A6FF" alt="HuggingFace"/>
  <img src="https://img.shields.io/badge/XGBoost-0D1117?style=for-the-badge&logo=scikitlearn&logoColor=58A6FF" alt="XGBoost"/>
  <img src="https://img.shields.io/badge/CUDA-0D1117?style=for-the-badge&logo=nvidia&logoColor=58A6FF" alt="CUDA"/>
</p>
<p align="center">
  <img src="https://img.shields.io/badge/Linux-0D1117?style=for-the-badge&logo=linux&logoColor=58A6FF" alt="Linux"/>
  <img src="https://img.shields.io/badge/Docker-0D1117?style=for-the-badge&logo=docker&logoColor=58A6FF" alt="Docker"/>
  <img src="https://img.shields.io/badge/Git-0D1117?style=for-the-badge&logo=git&logoColor=58A6FF" alt="Git"/>
  <img src="https://img.shields.io/badge/GitHub%20Actions-0D1117?style=for-the-badge&logo=githubactions&logoColor=58A6FF" alt="GitHub Actions"/>
</p>

## Competitive programming

Codeforces Expert, max rating 1803.
Round 1070: global rank 279 of 13,000+.
Round 1044: global rank 653 of 16,000+.
[codeforces.com/profile/Varun301004](https://codeforces.com/profile/Varun301004)

<br/>

## GitHub activity

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=Joker2841&show_icons=true&hide_border=true&bg_color=0D1117&title_color=58A6FF&icon_color=58A6FF&text_color=C9D1D9&border_radius=10&count_private=true" alt="GitHub Stats"/>
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Joker2841&layout=compact&hide_border=true&bg_color=0D1117&title_color=58A6FF&text_color=C9D1D9&border_radius=10" alt="Top Languages"/>
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=Joker2841&hide_border=true&background=0D1117&ring=58A6FF&fire=58A6FF&currStreakLabel=58A6FF&sideLabels=C9D1D9&currStreakNum=C9D1D9&sideNums=C9D1D9&dates=8B949E&border_radius=10" alt="GitHub Streak"/>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/Joker2841/Joker2841/output/github-contribution-grid-snake-dark.svg" alt="contribution snake"/>
</p>

<br/>

## What I read

A short list of what actually shaped how I think and work, split between systems papers and everything else.

**Papers:** The Log-Structured Merge-Tree (O'Neil et al.), Efficient ANN search using HNSW (Malkov and Yashunin), Dynamo (DeCandia et al.), The Google File System (Ghemawat et al.)

**Books:** Designing Data-Intensive Applications (Kleppmann), Database Internals (Petrov), Thinking, Fast and Slow (Kahneman), Atomic Habits (Clear), Deep Work (Newport)

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=0:0D1117,100:58A6FF&height=3&section=header" alt="divider"/>
</p>

<h2 align="center">Say hello</h2>

<p align="center">
  <a href="mailto:jokerbj2841@gmail.com"><img src="https://img.shields.io/badge/Email-0D1117?style=for-the-badge&logo=gmail&logoColor=58A6FF&labelColor=0D1117" alt="Email"/></a>
  <a href="https://www.linkedin.com/in/sai-girish-anga"><img src="https://img.shields.io/badge/LinkedIn-0D1117?style=for-the-badge&logo=linkedin&logoColor=58A6FF&labelColor=0D1117" alt="LinkedIn"/></a>
  <a href="https://tensen.dev"><img src="https://img.shields.io/badge/Blog-tensen.dev-0D1117?style=for-the-badge&logo=hashnode&logoColor=58A6FF&labelColor=0D1117" alt="Blog"/></a>
</p>
