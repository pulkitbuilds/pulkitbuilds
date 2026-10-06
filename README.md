<h1 align="center">👋 Hi, I'm Pulkit Sharma</h1>

<p align="center">
  🤖 AI/ML Engineer | Generative AI • RAG • Machine Learning • Python
</p>

<p align="center">
  <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&pause=1000&center=true&vCenter=true&width=600&lines=RAG+%26+Generative+AI+Systems;Real-Time+Audio+ML+%26+Deepfake+Voice+Detection;Full-Stack+AI+Apps+%7C+System+Design" alt="Typing SVG" />
</p>

<p align="center">
  <a href="https://pulkit-sharma-portfolio.vercel.app"><img src="https://img.shields.io/badge/Portfolio-000000?style=for-the-badge&logo=vercel&logoColor=white" /></a>
  <a href="https://www.linkedin.com/in/pulkit-sharma-319a2b314"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" /></a>
  <a href="mailto:pulkitsharma02345@gmail.com"><img src="https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white" /></a>
  <img src="https://komarev.com/ghpvc/?username=pulkitbuilds&color=blue&style=for-the-badge" />
</p>

---

## 👨‍💻 About Me

- 🎓 3rd-year B.Tech CSE (AI & ML) at **Career Point University, Kota** | CGPA **9.94+**
- 🏅 **AWS Certified AI Practitioner**
- 🥇 1st place, internal hackathon at CPU | Gold medal, IEEE Debate & Presentation
- 🏛️ President, **IPR Cell** at Career Point University
- 🌱 Currently learning: Generative AI, AI Agents, MLOps
- 🎯 Goal: build AI systems that solve real problems, and grow into a top-tier AI/ML engineering role

---

## 🖥️ Tech Stack

**Languages**

![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=cplusplus&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=postgresql&logoColor=white)

**AI / ML / Generative AI**

![PyTorch](https://img.shields.io/badge/PyTorch-EE4C2C?style=for-the-badge&logo=pytorch&logoColor=white)
![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/scikit--learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)
![OpenCV](https://img.shields.io/badge/OpenCV-5C3EE8?style=for-the-badge&logo=opencv&logoColor=white)
![Hugging Face](https://img.shields.io/badge/Sentence--Transformers-FFD21E?style=for-the-badge&logo=huggingface&logoColor=black)
![NVIDIA](https://img.shields.io/badge/NVIDIA_NIM-76B900?style=for-the-badge&logo=nvidia&logoColor=white)

**Backend, Cloud & Databases**

![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=for-the-badge&logo=fastapi&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-232F3E?style=for-the-badge&logo=amazonwebservices&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3ECF8E?style=for-the-badge&logo=supabase&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)

**Frontend & Tools**

![React](https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=for-the-badge&logo=vite&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)

**Also:** ChromaDB • BM25 • Librosa • Embeddings • Semantic Search • Hybrid Retrieval • REST APIs • **System Design**

---

## 🚀 Featured Projects

| Project | What it does | Tech |
|---|---|---|
| 🎙️ [**VoiceGuardAI**](https://github.com/pulkitbuilds/voiceguard2-) · [Live](https://voiceguard2.vercel.app) | Real-time platform that detects and prevents voice-cloning impersonation attacks | Python, Librosa, ML classification, Vercel |
| 📚 [**Evidentia**](https://github.com/pulkitbuilds/Evidentia-Evidence-first-editor) | Evidence-first editor backed by a hybrid RAG pipeline that grounds output in source documents | ChromaDB, BM25, sentence-transformers (`bge-small-en-v1.5`) |
| 🧑‍🎓 [**Face Attendance System**](https://github.com/pulkitbuilds/Facial_Attendence) | Face-recognition attendance web app with admin and read-only student roles | Next.js, Supabase, face-api.js, Vercel |

---

## 🏗️ System Design

High-level architecture of each project.

### 🎙️ VoiceGuardAI: real-time voice-clone detection

```mermaid
flowchart LR
    A[Audio input] --> B[Preprocessing]
    B --> C[Acoustic feature extraction<br/>Librosa]
    C --> D[ML classifier]
    D --> E{Real or<br/>cloned voice?}
    E -->|Genuine| F[Allow]
    E -->|Synthetic| G[Flag / prevent impersonation]
    D -.-> H[Web app on Vercel]
```

**Key ideas:** end-to-end audio ML pipeline, signal processing, low-latency inference, deployed as a live web app.

### 📚 Evidentia: evidence-first hybrid RAG

```mermaid
flowchart LR
    Q[User query] --> E[Embedding<br/>BAAI/bge-small-en-v1.5]
    Q --> K[Keyword search<br/>BM25]
    E --> V[Dense search<br/>ChromaDB]
    V --> R[Hybrid ranking]
    K --> R
    R --> G[Evidence-grounded<br/>response]
    D[(Source documents)] --> V
    D --> K
```

**Key ideas:** dense + sparse retrieval fused into one ranking, so answers stay tied to real source evidence instead of unsupported generation.

### 🧑‍🎓 Face Attendance System

```mermaid
flowchart LR
    C[Camera / browser] --> F[face-api.js<br/>face detection + recognition]
    F --> N[Next.js app]
    N --> S[(Supabase<br/>database + auth)]
    S --> A[Admin role<br/>full access]
    S --> T[Student role<br/>read-only]
    N --> V[Vercel deployment]
```

**Key ideas:** role-based access control, client-side face recognition, managed backend.

---

## 🏆 Achievements & Certifications

- 🥇 1st Place: Internal Hackathon, Career Point University
- 🥇 Gold Medal: IEEE Debate & Presentation
- 🥇 Gold Medal: University Table Tennis Event
- 🎓 Certificate of Excellence: Academic Achievement
- ☁️ AWS Certified AI Practitioner
- 📊 Google Data Analytics Professional Certificate
- 🤖 Machine Learning Certification (Udemy)
- 🤖 Machine Learning / AI Certification (IIT Bombay Techfest)

---

## 📊 GitHub Stats

<p align="center">
  <img height="170" src="https://github-readme-stats.vercel.app/api?username=pulkitbuilds&show_icons=true&theme=radical&hide_border=true" />
  <img height="170" src="https://github-readme-stats.vercel.app/api/top-langs/?username=pulkitbuilds&layout=compact&theme=radical&hide_border=true" />
</p>

<p align="center">
  <img src="https://streak-stats.demolab.com?user=pulkitbuilds&theme=radical&hide_border=true" />
</p>

---

<p align="center">
  💡 <i>"Learn. Build. Iterate. Repeat."</i>
</p>
