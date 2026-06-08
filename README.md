<div align="center">

```
 █████╗ ██╗   ██╗ █████╗     ██╗   ██╗ ██████╗ ██╗   ██╗███████╗███████╗███████╗██╗
██╔══██╗╚██╗ ██╔╝██╔══██╗    ╚██╗ ██╔╝██╔═══██╗██║   ██║██╔════╝██╔════╝██╔════╝██║
███████║ ╚████╔╝ ███████║     ╚████╔╝ ██║   ██║██║   ██║███████╗███████╗█████╗  ██║
██╔══██║  ╚██╔╝  ██╔══██║      ╚██╔╝  ██║   ██║██║   ██║╚════██║╚════██║██╔══╝  ██║
██║  ██║   ██║   ██║  ██║       ██║   ╚██████╔╝╚██████╔╝███████║███████║██║     ██║
╚═╝  ╚═╝   ╚═╝   ╚═╝  ╚═╝       ╚═╝    ╚═════╝  ╚═════╝ ╚══════╝╚══════╝╚═╝     ╚═╝
```

**AI & Digital Trust Engineering · ENSA Fès, Morocco**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-aya--youssfi-0A66C2?style=flat-square&logo=linkedin&logoColor=white)](https://linkedin.com/in/aya-youssfi)
[![GitHub](https://img.shields.io/badge/GitHub-ayayoussfiii-181717?style=flat-square&logo=github&logoColor=white)](https://github.com/ayayoussfiii)
[![Email](https://img.shields.io/badge/Email-aya.youssfi%40usmba.ac.ma-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:aya.youssfi@usmba.ac.ma)
[![Status](https://img.shields.io/badge/Status-Open%20to%20Internships-22d3a5?style=flat-square)](https://github.com/ayayoussfiii)
[![Oracle OCI](https://img.shields.io/badge/Oracle%20OCI%20AI-In%20Progress-F80000?style=flat-square&logo=oracle&logoColor=white)](https://github.com/ayayoussfiii)
[![Views](https://komarev.com/ghpvc/?username=ayayoussfiii&color=7c6bff&style=flat-square&label=profile+views)](https://github.com/ayayoussfiii)

</div>

---

```python
class AyaYoussfi:
    school   = "ENSA Fès — Cycle Ingénieur · AI & Digital Trust (2024–2026)"
    focus    = ["Explainable AI", "RAG Systems", "AI Safety", "Real-Time ML"]
    stack    = ["Python", "PyTorch", "LangChain", "Kafka", "SHAP", "Docker", "React"]
    certs    = ["Oracle OCI AI (in progress)", "Cisco CTM", "Cisco NET", "UM6P IIoT"]
    looking  = ["Internship", "Research Collaboration", "Open Source"]
    motto    = "Build systems that explain themselves."
```

---

## `01` &nbsp; Featured Projects

<table>
<tr>
<td valign="top" width="50%">

![](https://img.shields.io/badge/HIDS%20·%20Real--Time%20ML-7c6bff?style=flat-square&logoColor=white)

**🛡️ NetGuard IDS**

Real-time host-based intrusion detection on the **BETH Dataset** (NeurIPS 2021) — 8M+ kernel syscall events from 23 real AWS honeypots. Isolation Forest + XGBoost + SHAP + RAG over MITRE ATT&CK.

```python
# BETH — 8M+ events · 23 AWS honeypots
anomaly  = IsolationForest().fit(X_benign)
classify = XGBoost().fit(X_labelled)
explain  = shap.TreeExplainer(classify)
report   = rag.query(mitre_attack, alert)
```

![](https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apache-kafka)
![](https://img.shields.io/badge/SHAP-7c6bff?style=flat-square)
![](https://img.shields.io/badge/MITRE_ATT%26CK-CC0000?style=flat-square)
![](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi)
![](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![](https://img.shields.io/badge/ChromaDB-5b8dee?style=flat-square)

</td>
<td valign="top" width="50%">

![](https://img.shields.io/badge/AI%20Safety%20·%20Streaming-f87171?style=flat-square&logoColor=white)

**⚡ Real-Time Jailbreak Detection**

DistilBERT classifier streamed over Apache Pulsar. Hot-swap model watcher for zero-downtime updates. Adversarial prompt detection at sub-100ms latency.

```python
# streaming adversarial prompt classifier
stream = PulsarConsumer(topic="prompts")
model  = AutoModel.load(hot_swap=True)
label  = model.classify(stream.next())
# < 100ms end-to-end latency
```

![](https://img.shields.io/badge/DistilBERT-f87171?style=flat-square)
![](https://img.shields.io/badge/Apache%20Pulsar-188FFF?style=flat-square&logo=apache&logoColor=white)
![](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logo=pytorch&logoColor=white)
![](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logoColor=black)

</td>
</tr>
<tr>
<td valign="top" width="50%">

![](https://img.shields.io/badge/Fraud%20Detection%20·%20XAI-a78bfa?style=flat-square&logoColor=white)

**💳 Credit Card Fraud · HDBSCAN**

30k clients · HDBSCAN segmentation → per-cluster Gradient Boosting → SMOTE oversampling → SHAP per-cluster explainability · Flask REST API · deployed on Vercel.

```python
clusters  = HDBSCAN().fit_predict(X)
models    = {c: GBM().fit(X[c]) for c in clusters}
shap_vals = {c: TreeExplainer(m) for c, m in models}
api       = Flask().expose(models, shap_vals)
```

![](https://img.shields.io/badge/HDBSCAN-a78bfa?style=flat-square)
![](https://img.shields.io/badge/GBM-8b3fd4?style=flat-square)
![](https://img.shields.io/badge/SMOTE-7c35bb?style=flat-square)
![](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask)
![](https://img.shields.io/badge/Vercel-000000?style=flat-square&logo=vercel)

</td>
<td valign="top" width="50%">

![](https://img.shields.io/badge/AI%20Security%20·%20Proxy-38bdf8?style=flat-square&logoColor=white)

**🏭 GuardianAI + ChurnAI**

FastAPI AI security proxy with 3-layer middleware pipeline (auth, prompt filter, response audit). Paired with ChurnAI: XGBoost churn classifier + SHAP + LLM-generated personalised retention strategies.

```python
app = FastAPI()
app.add_middleware(AuthGuard)
app.add_middleware(PromptFilter)
app.add_middleware(ResponseAudit)
# + structured pytest suite · polished README
```

![](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi)
![](https://img.shields.io/badge/XGBoost-e8a838?style=flat-square)
![](https://img.shields.io/badge/LangChain-5b8dee?style=flat-square)
![](https://img.shields.io/badge/pytest-0A9EDC?style=flat-square&logo=pytest&logoColor=white)

</td>
</tr>
<tr>
<td valign="top" width="50%">

![](https://img.shields.io/badge/RAG%20·%20Flask%20API-22d3a5?style=flat-square&logoColor=black)

**📦 RAG Pipeline at ALTEN** *(internship)*

Production RAG pipeline with Flask API. Vector retrieval + LLM-grounded answers over internal documentation.

```python
embedder    = SentenceTransformer("all-MiniLM-L6-v2")
vectorstore = Chroma(embedder)
chain       = RetrievalQA(llm, vectorstore)
api         = Flask().expose(chain)
```

![](https://img.shields.io/badge/LangChain-5b8dee?style=flat-square)
![](https://img.shields.io/badge/ChromaDB-22d3a5?style=flat-square)
![](https://img.shields.io/badge/Flask-000000?style=flat-square&logo=flask)
![](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logoColor=black)

</td>
<td valign="top" width="50%">

![](https://img.shields.io/badge/Embedded%20AI%20·%20IoT-f59e0b?style=flat-square&logoColor=black)

**🦯 Smart Belt for Visually Impaired**

Arduino + GPS + ultrasonic sensors · Real-time obstacle detection · Haptic feedback navigation at the edge · no cloud dependency.

```c
while (true) {
  d = ultrasonic.read();
  if (d < THRESHOLD)
    haptic.pulse(map(d, 0, MAX, 255, 0));
  gps.track(location);
}
```

![](https://img.shields.io/badge/Arduino-00979D?style=flat-square&logo=arduino&logoColor=white)
![](https://img.shields.io/badge/IoT-f59e0b?style=flat-square)
![](https://img.shields.io/badge/GPS-1a7a38?style=flat-square)
![](https://img.shields.io/badge/Embedded-145c2a?style=flat-square)

</td>
</tr>
</table>

---

## `02` &nbsp; Stack

<table>
<tr>
<td valign="top" width="25%">

**AI · ML · XAI**
```
Python        ████████ 97%
PyTorch       ███████░ 82%
scikit-learn  ███████░ 85%
XGBoost       ███████░ 88%
SHAP          ███████░ 80%
TensorFlow    ██████░░ 75%
```

</td>
<td valign="top" width="25%">

**NLP · LLMs · RAG**
```
LangChain     ███████░ 78%
HuggingFace   ███████░ 80%
ChromaDB      ██████░░ 72%
DistilBERT    ██████░░ 75%
RAG Systems   █████░░░ 70%
Transformers  ██████░░ 73%
```

</td>
<td valign="top" width="25%">

**Infra · Backend**
```
Docker        ███████░ 80%
FastAPI       ███████░ 85%
Flask         ███████░ 85%
Kafka         ██████░░ 70%
PostgreSQL    ██████░░ 72%
Apache Pulsar █████░░░ 65%
```

</td>
<td valign="top" width="25%">

**Frontend · Data**
```
React         ███████░ 72%
Tailwind      ███████░ 75%
Pandas/NumPy  ████████ 92%
SQL           ██████░░ 78%
Java          █████░░░ 65%
Bash          █████░░░ 68%
```

</td>
</tr>
</table>

---

## `03` &nbsp; Certifications

<table>
<tr>
<td align="center" width="25%">
  <img src="https://img.shields.io/badge/OCI%20AI-F80000?style=for-the-badge&logo=oracle&logoColor=white"/><br/><br/>
  <sub><b>Generative AI Professional</b></sub><br/>
  <sub>Oracle · In progress</sub>
</td>
<td align="center" width="25%">
  <img src="https://img.shields.io/badge/CTM-1BA0D7?style=for-the-badge&logo=cisco&logoColor=white"/><br/><br/>
  <sub><b>Cyber Threat Management</b></sub><br/>
  <sub>Cisco</sub>
</td>
<td align="center" width="25%">
  <img src="https://img.shields.io/badge/NET-1BA0D7?style=for-the-badge&logo=cisco&logoColor=white"/><br/><br/>
  <sub><b>Network Technician</b></sub><br/>
  <sub>Cisco</sub>
</td>
<td align="center" width="25%">
  <img src="https://img.shields.io/badge/IIoT-00A651?style=for-the-badge&logoColor=white"/><br/><br/>
  <sub><b>Industrial IoT</b></sub><br/>
  <sub>UM6P</sub>
</td>
</tr>
</table>

---

## `04` &nbsp; GitHub Activity

<p align="center">
  <img src="https://img.shields.io/badge/Contributions-298-7c6bff?style=for-the-badge&logoColor=white"/>
  &nbsp;
  <img src="https://img.shields.io/badge/Projects-6+-22d3a5?style=for-the-badge&logoColor=white"/>
  &nbsp;
  <img src="https://img.shields.io/badge/Active%20Since-Nov%202025-f59e0b?style=for-the-badge&logoColor=black"/>
</p>

<p align="center">
  <img src="https://github-readme-activity-graph.vercel.app/graph?username=ayayoussfiii&theme=react-dark&hide_border=true&area=true&color=7c6bff&line=7c6bff&point=a78bfa&area_color=7c6bff" width="100%"/>
</p>

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=ayayoussfiii&show_icons=true&theme=tokyonight&hide_border=true&bg_color=0d0d14&title_color=a78bfa&icon_color=7c6bff&text_color=e2e2f0&ring_color=7c6bff" height="160"/>
  &nbsp;
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=ayayoussfiii&layout=compact&theme=tokyonight&hide_border=true&bg_color=0d0d14&title_color=a78bfa&text_color=e2e2f0&langs_count=6" height="160"/>
</p>

---

<div align="center">
  <i>"Build systems that explain themselves."</i>
  <br/><br/>
  <sub>Open to internships · research collaborations · open source · <a href="mailto:aya.youssfi@usmba.ac.ma">aya.youssfi@usmba.ac.ma</a></sub>
</div>
