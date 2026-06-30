<!-- Hero banner -->
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,20,30&height=200&section=header&text=Anga%20Sai%20Girish&fontSize=56&fontColor=ffffff&fontAlignY=38&desc=Software%20Engineer%20%C2%B7%20Backend%20%C2%B7%20Systems%20%C2%B7%20Applied%20AI&descSize=18&descAlignY=60&animation=fadeIn" alt="header"/>
</p>

<!-- Typing animation (compact, won't cut off) -->
<p align="center">
  <a href="https://github.com/Joker2841">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=22&duration=2800&pause=900&color=58A6FF&center=true&vCenter=true&width=600&lines=Software+Engineer+%E2%80%94+IIT+Guwahati+CSE+'26;Backend+%C2%B7+Systems+%C2%B7+Applied+AI;Codeforces+Expert+%E2%80%94+max+1803;Available+immediately+for+SDE+roles" alt="Typing SVG"/>
  </a>
</p>

<!-- Primary badges -->
<p align="center">
  <a href="https://tensen.dev"><img src="https://img.shields.io/badge/Blog-tensen.dev-FF7139?style=for-the-badge&logo=substack&logoColor=white" alt="Blog"/></a>
  <a href="https://www.linkedin.com/in/sai-girish-anga"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="https://codeforces.com/profile/Varun301004"><img src="https://img.shields.io/badge/Codeforces%20Expert-1803-1F8ACB?style=for-the-badge&logo=codeforces&logoColor=white" alt="Codeforces"/></a>
  <a href="mailto:jokerbj2841@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
</p>

<!-- Tertiary stats -->
<p align="center">
  <img src="https://komarev.com/ghpvc/?username=Joker2841&style=flat-square&color=58A6FF&label=Profile+Views" alt="Profile Views"/>
  <img src="https://img.shields.io/github/followers/Joker2841?style=flat-square&color=58A6FF&labelColor=0D1117" alt="Followers"/>
  <img src="https://img.shields.io/badge/Open%20to-SDE%20%2F%20Backend%20%2F%20Infra-success?style=flat-square&labelColor=0D1117" alt="Open to work"/>
</p>

<br/>

<!-- ────────────────────────────────────────────────────────────── -->

## <samp>About me</samp>

I'm a 2026 CSE graduate from **IIT Guwahati**. I work across backend systems and applied AI, and I'm most interested in problems where reliability and performance actually matter — storage internals, distributed systems, LLM infrastructure, the layers underneath the products people use.

```ts
const sai = {
    role:         "Software Engineer (2026 grad)",
    school:       "IIT Guwahati, Computer Science",
    focus:        ["Storage systems", "LLM evaluation", "Backend"],
    languages:    ["Rust", "C++", "Python", "Java"],
    currently:    "Building Sastran — a crash-safe storage engine",
    competitive:  "Codeforces Expert (max 1803)",
    writing_at:   "tensen.dev",
    open_to:      "Full-time SDE / Backend / Infrastructure roles",
    based_in:     "India",
    availability: "Immediate"
};
```

The fastest way to know what I work on is to look at what I build — scroll down.

<br/>

<!-- ────────────────────────────────────────────────────────────── -->

## <samp>Right now</samp>

<p>
  <img src="https://img.shields.io/badge/Building-Sastran%20storage%20engine-orange?style=for-the-badge&logo=rust&logoColor=white&labelColor=0D1117" alt="Building"/>
  <img src="https://img.shields.io/badge/Interviewing-Full--time%20SDE%20roles-58A6FF?style=for-the-badge&logo=googlemeet&logoColor=white&labelColor=0D1117" alt="Interviewing"/>
</p>
<p>
  <img src="https://img.shields.io/badge/Prototyping-coherence%20(Cognee%20hackathon)-9B59B6?style=for-the-badge&logo=neo4j&logoColor=white&labelColor=0D1117" alt="Prototyping"/>
  <img src="https://img.shields.io/badge/Writing-tensen.dev-FF7139?style=for-the-badge&logo=hashnode&logoColor=white&labelColor=0D1117" alt="Writing"/>
  <img src="https://img.shields.io/badge/Climbing-Codeforces%20toward%20CM-1F8ACB?style=for-the-badge&logo=codeforces&logoColor=white&labelColor=0D1117" alt="Climbing"/>
</p>

<br/>

<!-- ────────────────────────────────────────────────────────────── -->

## <samp>Featured projects</samp>

<table>
<tr>
<td width="50%" valign="top">

<h3>🦀 Sastran</h3>
<p><em>Crash-safe storage engine in Rust</em></p>

Unified key-value and vector storage. LSM-tree for KV, HNSW for ANN search, one durability story across both.

- WAL with CRC-checked records, fsync ordering
- Leveled compaction over block-structured SSTables
- Per-SSTable bloom filters: **~28× speedup** on absent-key lookups (2.63µs → 94ns)
- HNSW with crash-consistent snapshot-and-replay recovery
- Recall@10 > 0.80 after **30% vector deletion** via neighbor repair
- 8-bit scalar quantization: **4× compression at 96.2% recall**
- ~3,000 lines Rust · ~190 tests · **zero unsafe**

`Rust` `LSM-Tree` `HNSW` `WAL` `Criterion`

<a href="https://github.com/Joker2841/sastran"><img src="https://img.shields.io/badge/View%20repository-181717?style=flat-square&logo=github&logoColor=white" alt="repo"/></a>

</td>
<td width="50%" valign="top">

<h3>🧠 DocuMind</h3>
<p><em>Full-stack RAG document assistant</em></p>

Production-style RAG system supporting semantic Q&A across PDFs, DOCX, HTML, Markdown.

- FastAPI backend, React frontend, PostgreSQL
- GPU-accelerated retrieval with BAAI/bge-large-en-v1.5
- FAISS vector search + custom heuristic filtering
- Real-time updates over WebSockets
- Containerized with Docker, PWA support
- **Sub-10ms** semantic retrieval latency

`FastAPI` `React` `PostgreSQL` `FAISS` `PyTorch CUDA` `Docker`

<a href="https://github.com/Joker2841/document-qa-rag-new"><img src="https://img.shields.io/badge/View%20repository-181717?style=flat-square&logo=github&logoColor=white" alt="repo"/></a>

</td>
</tr>
<tr>
<td width="50%" valign="top">

<h3>🎯 RAG-Aware LLM Routing</h3>
<p><em>B.Tech thesis · Prof. Amit Awekar</em></p>

Cost-aware routing system that dynamically selects between small and large language models per query.

- Routes 2B vs 30B models on complexity + confidence signals
- 22 predictive features, cost-sensitive XGBoost
- Interaction-based signals catch small-model failures
- **~41% inference-cost reduction**
- **93.3% answer quality preserved**
- Evaluation pipeline over **1,500 queries**, 50+ GPU oracle hours

`Python` `XGBoost` `PyTorch` `LLMs` `RAG`

<a href="https://github.com/Joker2841/rag-aware-routing"><img src="https://img.shields.io/badge/View%20repository-181717?style=flat-square&logo=github&logoColor=white" alt="repo"/></a>

</td>
<td width="50%" valign="top">

<h3>😏 Sarcasm Detection (ACE 2+)</h3>
<p><em>NLP / Deep Learning course project</em></p>

Fine-tuned DeBERTa-v3 for sarcasm detection with custom affective-feature fusion.

- 94.77% macro-F1 on 28K news headlines
- **Exceeds COLING 2020 benchmark** (+2.56 F1)
- Custom Sentiment Incongruity Score (SIS)
- 10-dim Affective Feature Embedding (AFE)
- Gated Fusion layer, full 4-variant ablation study

`PyTorch` `DeBERTa-v3` `HuggingFace` `NLP`

<a href="https://bit.ly/sg_sarcasm"><img src="https://img.shields.io/badge/View%20repository-181717?style=flat-square&logo=github&logoColor=white" alt="repo"/></a>

</td>
</tr>
<tr>
<td width="50%" valign="top">

<h3>🔎 Redrob — Intelligent Candidate Discovery</h3>
<p><em>Track 01 hackathon · CPU-fast ranking with LLM coherence</em></p>

Ranks **100,000 candidates** against a Senior ML/AI JD via structural signals + LLM-grounded coherence checking. 5-stage pipeline: relevance floor → honeypot gate → JD disqualifier → calibrated scorer × multipliers.

- **LLM re-tasked**: qwen2.5:7b (Ollama) shifted from tier-scorer to narrow coherence checker after templated prose inflated tier scores
- Structural trap detection: tool anachronisms, narrative inconsistencies, domain mismatches
- Empirical signal validation — dropped fps weight, dup-detection after measuring against full 100K pool
- Two-pass design with offline LLM precompute and CPU-only ranking
- **NDCG@10 = 0.929**, NDCG@50 = 0.978 on hand-built gold set
- **< 5 min for 100K candidates**, no network, MIT licensed

`Python` `Ollama` `LLM-as-judge` `Empirical eval`

<a href="https://github.com/Joker2841/redrob-ranker"><img src="https://img.shields.io/badge/View%20repository-181717?style=flat-square&logo=github&logoColor=white" alt="repo"/></a>

</td>
<td width="50%" valign="top">

<h3>📂 More work</h3>
<p><em>A few other things I've built</em></p>

- **NIDS** — Real-time network intrusion detection (1-3K packets/sec via BPF + multi-threaded Python). The project where I debugged Python's GIL bottleneck firsthand. → [repo](https://github.com/Joker2841/NIDS)
- **Runway** — AI agent that helps you finish commitments before deadlines, not just remember them. Built with Gemini on Google AI Studio. → [repo](https://github.com/Joker2841/Runway)
- **SkyConnect** — MERN-stack flight booking platform with REST API, automated notifications (node-cron + Nodemailer), admin panel.
- **Codeforces archive** + **Gridlock 2.0 hackathon** — competitive programming climb from newbie to Expert; Bengaluru Traffic Police × Flipkart traffic demand prediction (~89.1 leaderboard).

All public repos at <a href="https://github.com/Joker2841?tab=repositories">my repositories page →</a>

</td>
</tr>
</table>

<br/>

<!-- ────────────────────────────────────────────────────────────── -->

## <samp>How I work</samp>

A few principles I've actually learned from building these — not borrowed from somewhere.

> **Measure before optimizing.** The 28× bloom filter speedup in Sastran came from writing the benchmark in Criterion *before* writing the optimization. The 41% routing cost reduction came from labeling 1,500 queries with GPU oracle data before training a router. In Redrob I dropped several intuitive signals — keyword density, duplicate-description detection, education date-ordering — to zero after measuring they had no ranking value across 100K candidates. I learned this the hard way enough times that it's now reflex.

> **Learn by building.** Rust at depth came from building Sastran, not from a course. HNSW came from reading the Malkov–Yashunin paper and implementing it, not from a library wrapper. The fastest path to understanding something is usually to ship it.

> **Comfortable being wrong.** From competitive programming, my code gets judged objectively against test cases every weekend. Disagreement and error feel like information, not threat.

> **Honest about scope.** Sastran is a single-node engine, not a distributed system. DocuMind is production-style, not battle-tested in production. I'd rather scope something small and finish it well than wave my hands at something I haven't built.

<br/>

<!-- ────────────────────────────────────────────────────────────── -->

## <samp>Tech stack</samp>

<table align="center">
<tr>
<td valign="top" width="50%">

<h4 align="center">🛠 Languages I reach for first</h4>
<p align="center">
  <img src="https://img.shields.io/badge/Rust-000000?style=for-the-badge&logo=rust&logoColor=white"/>
  <img src="https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white"/>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Java-ED8B00?style=for-the-badge&logo=openjdk&logoColor=white"/>
  <img src="https://img.shields.io/badge/SQL-CC2927?style=for-the-badge&logo=postgresql&logoColor=white"/>
  <img src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black"/>
</p>

<h4 align="center">⚙️ Backend &amp; APIs</h4>
<p align="center">
  <img src="https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white"/>
  <img src="https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white"/>
  <img src="https://img.shields.io/badge/Express-000000?style=for-the-badge&logo=express&logoColor=white"/>
  <img src="https://img.shields.io/badge/REST-005571?style=for-the-badge&logo=fastapi&logoColor=white"/>
  <img src="https://img.shields.io/badge/WebSockets-4353FF?style=for-the-badge&logo=socketdotio&logoColor=white"/>
</p>

<h4 align="center">💾 Data &amp; storage</h4>
<p align="center">
  <img src="https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white"/>
  <img src="https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white"/>
  <img src="https://img.shields.io/badge/MySQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white"/>
  <img src="https://img.shields.io/badge/FAISS-0467DF?style=for-the-badge&logo=meta&logoColor=white"/>
  <img src="https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white"/>
</p>

</td>
<td valign="top" width="50%">

<h4 align="center">🧠 ML &amp; AI</h4>
<p align="center">
  <img src="https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white"/>
  <img src="https://img.shields.io/badge/HuggingFace-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black"/>
  <img src="https://img.shields.io/badge/XGBoost-EB6E4B?style=for-the-badge&logo=scikit-learn&logoColor=white"/>
  <img src="https://img.shields.io/badge/CUDA-76B900?style=for-the-badge&logo=nvidia&logoColor=white"/>
  <img src="https://img.shields.io/badge/RAG-512BD4?style=for-the-badge&logo=openai&logoColor=white"/>
</p>

<h4 align="center">🐧 Systems &amp; DevOps</h4>
<p align="center">
  <img src="https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black"/>
  <img src="https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white"/>
  <img src="https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white"/>
  <img src="https://img.shields.io/badge/GitHub%20Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white"/>
  <img src="https://img.shields.io/badge/Criterion-A41E22?style=for-the-badge&logo=rust&logoColor=white"/>
</p>

<h4 align="center">🎨 Frontend (when needed)</h4>
<p align="center">
  <img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black"/>
  <img src="https://img.shields.io/badge/TailwindCSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white"/>
  <img src="https://img.shields.io/badge/Zustand-2D2D2D?style=for-the-badge&logo=react&logoColor=white"/>
</p>

</td>
</tr>
</table>

<br/>

<!-- ────────────────────────────────────────────────────────────── -->

## <samp>Competitive programming</samp>

I've competed on Codeforces since 2022. It's where I first learned to think about problems systematically and to take being wrong as information.

<table align="center">
<tr>
<td valign="top" width="50%" align="center">

<h4>🏆 Codeforces — Expert</h4>

<img src="https://img.shields.io/badge/Current%20Rating-1798-1F8ACB?style=for-the-badge&labelColor=0D1117"/>
<img src="https://img.shields.io/badge/Peak%20Rating-1803-FFD700?style=for-the-badge&labelColor=0D1117"/>

<br/><br/>

| Contest | Global Rank |
|--------:|:------------|
| Round 1070 | **279** / 13,000+ |
| Round 1044 | **653** / 16,000+ |

<a href="https://codeforces.com/profile/Varun301004"><img src="https://img.shields.io/badge/View%20profile-1F8ACB?style=flat-square&logo=codeforces&logoColor=white" alt="CF"/></a>

</td>
<td valign="top" width="50%" align="center">

<h4>🎓 Academic</h4>

<img src="https://img.shields.io/badge/JEE%20Advanced-AIR%201592-success?style=for-the-badge&labelColor=0D1117"/>
<br/>
<img src="https://img.shields.io/badge/JEE%20Main-AIR%201135-success?style=for-the-badge&labelColor=0D1117"/>

<br/><br/>

| Exam | Score |
|:-----|------:|
| AP EAPCET 2022 | State Rank **118** |
| Class XII (2022) | **93.2%** |
| Class X (2020) | **100%** |

</td>
</tr>
</table>

<br/>

<!-- ────────────────────────────────────────────────────────────── -->

## <samp>GitHub stats</samp>

<p align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=Joker2841&show_icons=true&hide_border=true&theme=tokyonight&include_all_commits=true&count_private=true&rank_icon=github" alt="GitHub Stats"/>
  <img height="170" src="https://github-readme-streak-stats.herokuapp.com/?user=Joker2841&hide_border=true&theme=dark&background=0D1117" alt="GitHub Streak"/>
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Joker2841&layout=compact&hide_border=true&theme=tokyonight&langs_count=8&card_width=480" alt="Top Languages"/>
</p>

<p align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=Joker2841&theme=darkhub&no-frame=true&no-bg=true&margin-w=6&row=1&column=7" alt="GitHub Trophies"/>
</p>

<details>
<summary><b>📈 Contribution activity graph</b></summary>
<br/>
<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=Joker2841&theme=tokyo-night&hide_border=true&area=true&custom_title=Contribution%20Activity" alt="Activity Graph"/>
</p>
</details>

<!-- Snake animation (requires GitHub Action setup — see README notes) -->
<p align="center">
  <img src="https://raw.githubusercontent.com/Joker2841/Joker2841/output/github-contribution-grid-snake-dark.svg" alt="snake animation"/>
</p>

<br/>

<!-- ────────────────────────────────────────────────────────────── -->

## <samp>What I read &amp; think about</samp>

Reading shapes how I work as much as building does. A short list of what's actually on my shelf — split between systems papers that inform my engineering and the broader books that shape how I think.

### 📄 Papers that inform my engineering

| Paper | Why it matters to me |
|:------|:---------------------|
| **The Log-Structured Merge-Tree** — O'Neil et al. | The foundation behind LevelDB, RocksDB, and Sastran's KV layer |
| **Efficient ANN search using HNSW** — Malkov & Yashunin | What Sastran's vector index implements |
| **Dynamo: Amazon's Highly Available Key-value Store** | For thinking about distribution, replication, and eventual consistency |
| **The Google File System** — Ghemawat et al. | Still the cleanest introduction to large-scale block storage |

### 📚 Engineering books

| Book | Why it matters to me |
|:-----|:---------------------|
| **Designing Data-Intensive Applications** — Kleppmann | The textbook I wish every backend engineer read |
| **Database Internals** — Petrov | Dense but excellent on storage engines specifically |

### 🧭 Beyond engineering — how I think and work

| Book | Why it matters to me |
|:-----|:---------------------|
| **Thinking, Fast and Slow** — Kahneman | The book that changed how I treat my own intuitions |
| **Deep Work** — Cal Newport | Why I protect long uninterrupted blocks for hard problems |
| **Atomic Habits** — James Clear | Systems over goals — the framing that actually changed my daily work |
| **Make It Stick** — Brown, Roediger, McDaniel | Evidence-based learning, written for technical readers |
| **Clear Thinking** — Shane Parrish | On catching the moments where defaults make decisions for you |
| **Man's Search for Meaning** — Viktor Frankl | The book I return to when work feels heavy |
| **Meditations** — Marcus Aurelius | Short, ancient, still the best operating manual I've found for a noisy mind |

<br/>

<!-- ────────────────────────────────────────────────────────────── -->

## <samp>Writing</samp>

I write occasionally at **[tensen.dev](https://tensen.dev)** — mostly notes on systems, what I'm learning, and the occasional deep-dive into something I built.

<p>
  <a href="https://tensen.dev"><img src="https://img.shields.io/badge/Read%20on-tensen.dev-FF7139?style=for-the-badge&logo=hashnode&logoColor=white&labelColor=0D1117" alt="Blog"/></a>
</p>

<br/>

<!-- ────────────────────────────────────────────────────────────── -->

## <samp>Let's talk</samp>

I'm open to full-time **SDE, backend, and infrastructure** roles, including AI / LLM platform work. Most interested in companies where the engineering bar is high and the work touches reliability, performance, or data at meaningful scale.

<p align="center">
  <a href="mailto:jokerbj2841@gmail.com"><img src="https://img.shields.io/badge/Email-jokerbj2841%40gmail.com-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"/></a>
  <a href="https://www.linkedin.com/in/sai-girish-anga"><img src="https://img.shields.io/badge/LinkedIn-Connect-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
  <a href="https://tensen.dev"><img src="https://img.shields.io/badge/Blog-tensen.dev-FF7139?style=for-the-badge&logo=hashnode&logoColor=white" alt="Blog"/></a>
  <a href="https://github.com/Joker2841"><img src="https://img.shields.io/badge/GitHub-Follow-181717?style=for-the-badge&logo=github&logoColor=white" alt="GitHub"/></a>
</p>

<p align="center">
  <sub>📍 Available immediately · Bengaluru / Hyderabad / Remote</sub>
</p>

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=12,20,30&height=120&section=footer&reversal=true" alt="footer"/>
</p>
