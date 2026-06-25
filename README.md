<h1 align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=28&duration=3000&pause=800&color=58A6FF&center=true&vCenter=true&width=720&lines=Hi%2C+I'm+Anga+Sai+Girish;Software+Engineer+%E2%80%94+Backend%2C+Systems%2C+Applied+AI;IIT+Guwahati+CSE+'26;Codeforces+Expert+(max+1803);Open+to+SDE+roles+%E2%80%94+available+immediately" alt="Typing SVG" />
</h1>

<p align="center">
  <a href="https://www.linkedin.com/in/sai-girish-anga"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="https://codeforces.com/profile/Varun301004"><img src="https://img.shields.io/badge/Codeforces%20Expert-1803-1F8ACB?style=for-the-badge&logo=codeforces&logoColor=white" alt="Codeforces"/></a>
  <a href="mailto:jokerbj2841@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
</p>

<p align="center">
  <img src="https://komarev.com/ghpvc/?username=Joker2841&style=for-the-badge&color=58A6FF&label=Profile+Views" alt="Profile Views"/>
  <img src="https://img.shields.io/github/followers/Joker2841?style=for-the-badge&color=58A6FF&labelColor=0D1117" alt="Followers"/>
</p>

---

## About me

I'm a 2026 CSE graduate from **IIT Guwahati**. I work across backend systems and applied AI, and I'm most interested in problems where reliability and performance actually matter — storage internals, distributed systems, LLM infrastructure, the layers underneath the products people use.

```text
const sai = {
    role:         "Software Engineer (2026 grad)",
    school:       "IIT Guwahati, Computer Science",
    focus:        ["Backend", "Storage systems", "Applied AI / RAG"],
    languages:    ["Rust", "C++", "Python", "Java"],
    currently:    "Building Sastran — a crash-safe storage engine",
    competitive:  "Codeforces Expert (max 1803)",
    open_to:      "Full-time SDE / Backend / Infrastructure roles",
    based_in:     "India",
    availability: "Immediate"
};
```

The fastest way to know what I work on is to look at what I build — scroll down for the projects.

---

## What I'm doing right now

- Building **Sastran**, a crash-safe unified KV + vector storage engine in Rust.
- Interviewing for full-time SDE and infrastructure roles for July 2026.
- Reading distributed-systems papers: GFS, Dynamo, Spanner, the LSM-tree literature.
- Occasionally sharpening on Codeforces — currently chasing Candidate Master.

---

## Featured projects

<table>
<tr>
<td width="50%" valign="top">

### Sastran
**Crash-safe storage engine in Rust**

Unified key-value and vector storage. LSM-tree for KV, HNSW for ANN search, one durability story across both.

- WAL with CRC-checked records, fsync ordering
- Leveled compaction over block-structured SSTables
- Per-SSTable bloom filters: **~28x speedup** on absent-key lookups (2.63µs → 94ns)
- HNSW with crash-consistent snapshot-and-replay recovery
- Recall@10 > 0.80 after **30% vector deletion** via neighbor repair
- 8-bit scalar quantization: **4x compression at 96.2% recall**
- ~3,000 lines Rust, ~190 tests, **zero unsafe code**

`Rust` `LSM-Tree` `HNSW` `WAL` `Criterion`

[**Repository →**](https://github.com/Joker2841/sastran)

</td>
<td width="50%" valign="top">

### DocuMind
**Full-stack RAG document assistant**

Production-style RAG system supporting semantic Q&A across PDFs, DOCX, HTML, Markdown.

- FastAPI backend, React frontend, PostgreSQL
- GPU-accelerated retrieval with BAAI/bge-large-en-v1.5
- FAISS vector search + custom heuristic filtering
- Real-time updates over WebSockets
- Containerized with Docker, PWA support
- **Sub-10ms** semantic retrieval latency

`FastAPI` `React` `PostgreSQL` `FAISS` `PyTorch CUDA` `Docker`

[**Repository →**](https://github.com/Joker2841/document-qa-rag-new)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### RAG-Aware LLM Routing
**B.Tech thesis (Prof. Amit Awekar)**

Cost-aware routing system that dynamically selects between small and large language models per query.

- Routes 2B vs 30B models on complexity + confidence signals
- 22 predictive features, cost-sensitive XGBoost
- Interaction-based signals catch small-model failures
- **~41% inference-cost reduction**
- **93.3% answer quality preserved**
- Evaluation pipeline over **1,500 queries**, 50+ GPU oracle hours

`Python` `XGBoost` `PyTorch` `LLMs` `RAG`

[**Repository →**](https://github.com/Joker2841/rag-aware-routing)

</td>
<td width="50%" valign="top">

### Sarcasm Detection (ACE 2+)
**NLP / Deep Learning course project**

Fine-tuned DeBERTa-v3 for sarcasm detection with custom affective-feature fusion.

- 94.77% macro-F1 on 28K news headlines
- **Exceeds COLING 2020 benchmark** (+2.56 F1)
- Custom Sentiment Incongruity Score (SIS)
- 10-dim Affective Feature Embedding (AFE)
- Gated Fusion layer, full 4-variant ablation study

`PyTorch` `DeBERTa-v3` `HuggingFace` `NLP`

[**Repository →**](https://bit.ly/sg_sarcasm)

</td>
</tr>
<tr>
<td width="50%" valign="top">

### Real-time NIDS
**Network Intrusion Detection System**

Real-time cybersecurity monitoring with BPF-optimized packet capture.

- Multi-threaded Python with BPF filters
- 1,000–3,000 packets/sec, <200ms alert latency
- 8 threat detection algorithms (SYN flood, port scan, ARP spoof, ICMP flood, LAND, etc.)
- Full-stack dashboard with live WebSocket updates
- Interactive threat visualizations in Plotly
- Geographic IP tracking, persistent SQLite

`Python` `BPF` `WebSockets` `SQLite` `Plotly`

[**Repository →**](https://github.com/Joker2841/NIDS)

</td>
<td width="50%" valign="top">

### More work

A few other things I've built or contributed to:

- **SkyConnect** — MERN-stack flight booking platform with REST API, automated notifications (node-cron + Nodemailer), and admin panel
- **Various Codeforces solutions** — competitive programming archive, ratings climbed from newbie to Expert
- **Hackathon work** — including Gridlock 2.0 (HackerEarth × Flipkart × Bengaluru Traffic Police) with leaderboard score ~89.1 on traffic-demand prediction

All public repos are linked from my [repositories page](https://github.com/Joker2841?tab=repositories).

</td>
</tr>
</table>

---

## How I work

A few principles I've actually learned from building these, not borrowed from somewhere:

**Measure before optimizing.** The 28x bloom filter speedup in Sastran came from writing the benchmark in Criterion *before* writing the optimization. The 41% routing cost reduction came from labeling 1,500 queries with GPU oracle data before training a router. I learned this the hard way enough times that it's now reflex.

**Learn by building.** Rust at depth came from building Sastran, not from a course. HNSW came from reading the Malkov–Yashunin paper and implementing it, not from a library wrapper. The fastest path to understanding something is usually to ship it.

**Comfortable being wrong.** From competitive programming, my code gets judged objectively against test cases every weekend. Disagreement and error feel like information, not threat.

**Honest about scope.** Sastran is a single-node engine, not a distributed system. DocuMind is production-style, not battle-tested in production. I'd rather scope something small and finish it well than wave my hands at something I haven't built.

---

## Tech stack

<h3>Languages I reach for first</h3>
<p>
<img src="https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white" alt="Rust"/>
<img src="https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white" alt="C++"/>
<img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python"/>
<img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java"/>
<img src="https://img.shields.io/badge/SQL-CC2927?style=for-the-badge&logo=postgresql&logoColor=white" alt="SQL"/>
<img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" alt="JavaScript"/>
</p>

<h3>Backend &amp; APIs</h3>
<p>
<img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white" alt="FastAPI"/>
<img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" alt="Node.js"/>
<img src="https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white" alt="Express"/>
<img src="https://img.shields.io/badge/REST-005571?style=for-the-badge&logo=fastapi&logoColor=white" alt="REST"/>
<img src="https://img.shields.io/badge/WebSockets-4353FF?style=for-the-badge&logo=socketdotio&logoColor=white" alt="WebSockets"/>
</p>

<h3>Data &amp; storage</h3>
<p>
<img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL"/>
<img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white" alt="MongoDB"/>
<img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL"/>
<img src="https://img.shields.io/badge/FAISS-0467DF?style=for-the-badge&logo=meta&logoColor=white" alt="FAISS"/>
<img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white" alt="Redis"/>
</p>

<h3>ML &amp; AI</h3>
<p>
<img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white" alt="PyTorch"/>
<img src="https://img.shields.io/badge/HuggingFace-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black" alt="HuggingFace"/>
<img src="https://img.shields.io/badge/XGBoost-EB6E4B?style=for-the-badge&logo=scikit-learn&logoColor=white" alt="XGBoost"/>
<img src="https://img.shields.io/badge/CUDA-76B900?style=for-the-badge&logo=nvidia&logoColor=white" alt="CUDA"/>
<img src="https://img.shields.io/badge/RAG-512BD4?style=for-the-badge&logo=openai&logoColor=white" alt="RAG"/>
</p>

<h3>Systems &amp; DevOps</h3>
<p>
<img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black" alt="Linux"/>
<img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white" alt="Docker"/>
<img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white" alt="Git"/>
<img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white" alt="GitHub Actions"/>
<img src="https://img.shields.io/badge/Criterion-A41E22?style=for-the-badge&logo=rust&logoColor=white" alt="Criterion"/>
</p>

<h3>Frontend (when needed)</h3>
<p>
<img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black" alt="React"/>
<img src="https://img.shields.io/badge/TailwindCSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white" alt="Tailwind"/>
<img src="https://img.shields.io/badge/Zustand-2D2D2D?style=for-the-badge&logo=react&logoColor=white" alt="Zustand"/>
</p>

---

## Competitive programming

I've competed on Codeforces since 2022. It's where I first learned to think about problems systematically and to take being wrong as information.

<table>
<tr>
<td valign="top" width="50%">

**Codeforces — Expert**
- Current rating: 1798 / Max: **1803**
- Round 1070: **Global Rank 279** (of 13,000+)
- Round 1044: **Global Rank 653** (of 16,000+)
- [Profile →](https://codeforces.com/profile/Varun301004)

</td>
<td valign="top" width="50%">

**Academic**
- JEE Advanced 2022: AIR **1592** (of 0.15M)
- JEE Main 2022: AIR **1135** (of 1M)
- AP EAPCET 2022: State Rank **118**
- Class XII: **93.2%**
- Class X: **100%**

</td>
</tr>
</table>

---

## GitHub stats

<p align="center">
  <img height="180" src="https://github-readme-stats.vercel.app/api?username=Joker2841&show_icons=true&hide_border=true&theme=tokyonight&include_all_commits=true&count_private=true" alt="GitHub Stats"/>
  <img height="180" src="https://github-readme-streak-stats.herokuapp.com/?user=Joker2841&hide_border=true&theme=tokyonight" alt="GitHub Streak"/>
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Joker2841&layout=compact&hide_border=true&theme=tokyonight&langs_count=8" alt="Top Languages"/>
</p>

<p align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=Joker2841&theme=tokyonight&no-frame=true&no-bg=true&margin-w=4&row=1" alt="GitHub Trophies"/>
</p>

<details>
<summary><b>Contribution graph</b></summary>
<br>
<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=Joker2841&theme=tokyo-night&hide_border=true&area=true" alt="Activity Graph"/>
</p>
</details>

---

## What I read &amp; think about

A short list of papers and books that have shaped how I think — not exhaustive, just the ones I'd actually recommend.

- **The Log-Structured Merge-Tree (LSM-Tree)** — O'Neil et al., the original paper behind LevelDB, RocksDB, and Sastran's KV layer
- **Efficient and robust approximate nearest neighbor search using HNSW** — Malkov &amp; Yashunin, what Sastran's vector index implements
- **Dynamo: Amazon's Highly Available Key-value Store** — for thinking about distribution, replication, and eventual consistency
- **The Google File System** — Ghemawat et al., still the cleanest introduction to large-scale block storage
- **Designing Data-Intensive Applications** — Kleppmann, the textbook I wish every backend engineer read
- **Database Internals** — Petrov, dense but excellent on storage engines specifically

---

## Let's talk

I'm open to full-time **SDE, backend, and infrastructure** roles, including AI / LLM platform work. Most interested in companies where the engineering bar is high and the work touches reliability, performance, or data at meaningful scale.

<p align="center">
  <a href="mailto:jokerbj2841@gmail.com"><img src="https://img.shields.io/badge/Email-jokerbj2841%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
  <a href="https://www.linkedin.com/in/sai-girish-anga"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="https://github.com/Joker2841"><img src="https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/></a>
</p>

<p align="center">
  <sub>Available immediately · Bengaluru / Hyderabad / Remote</sub>
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=6,11,20&height=120&section=footer&reversal=true" alt="footer"/>
</p>
