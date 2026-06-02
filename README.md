<div align="center">
<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0a0a0a,50:111111,100:0a0a0a&height=260&section=header&text=Aya%20Youssfi&fontSize=72&fontColor=ffffff&fontAlignY=44&fontAlign=50&desc=AI%20%26%20Digital%20Trust%20Engineering%20·%20ENSA%20Fès%2C%20Morocco&descAlignY=64&descSize=13&descColor=666666" width="100%"/>
</div>

<br/>

<div align="center">

![Typing SVG](https://readme-typing-svg.demolab.com?font=JetBrains+Mono&size=13&duration=3500&pause=1200&color=999999&center=true&vCenter=true&width=650&lines=ML+Pipelines+·+RAG+Systems+·+Explainable+AI+·+Real-Time+Inference;PyTorch+·+LangChain+·+HuggingFace+·+Apache+Pulsar+·+Docker;Open+to+internships+%26+research+collaborations+—+Fès%2C+Morocco)

</div>

<br/>

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-aya--youssfi-ffffff?style=flat-square&logo=linkedin&logoColor=black&labelColor=ffffff&color=ffffff)](https://linkedin.com/in/aya-youssfi)&ensp;[![Email](https://img.shields.io/badge/Email-aya.youssfi%40usmba.ac.ma-ffffff?style=flat-square&logo=gmail&logoColor=black&labelColor=ffffff&color=ffffff)](mailto:aya.youssfi@usmba.ac.ma)&ensp;[![GitHub](https://img.shields.io/badge/GitHub-ayayoussfiii-ffffff?style=flat-square&logo=github&logoColor=black&labelColor=ffffff&color=ffffff)](https://github.com/ayayoussfiii)&ensp;![Status](https://img.shields.io/badge/Status-Open%20to%20Internships-111111?style=flat-square&logoColor=white)

</div>

<br/>

---

<br/>

```
  ┌─ profile ──────────────────────────────────────────────────────────┐
  │                                                                     │
  │  name      →  Aya Youssfi                                          │
  │  school    →  ENSA Fès — Cycle Ingénieur · AI & Digital Trust      │
  │  focus     →  Explainable AI · RAG Systems · AI Safety             │
  │              Real-Time ML · Streaming Architectures                │
  │  stack     →  Python · PyTorch · LangChain · HuggingFace           │
  │              Apache Pulsar · Docker · SHAP · scikit-learn          │
  │  languages →  Python · Java · SQL · Bash                           │
  │  looking   →  Internship · Research Collaboration · Open Source    │
  │  motto     →  "Build systems that explain themselves."             │
  │                                                                     │
  └─────────────────────────────────────────────────────────────────── ┘
```

<br/>

---

<br/>

## Projects

<br/>

<table width="100%">
<tr>
<td width="4%" valign="top">
<br/><sub><code>01</code></sub>
</td>
<td width="46%" valign="top">

### Customer Churn + LLM Retention
*Machine Learning · Explainability · NLP*

End-to-end ML pipeline with **XGBoost** classifier, **SHAP** feature explainability, and **LLM-generated** personalised retention strategies. Streamlit dashboard for real-time business insights.

```python
model    = XGBoostClassifier()
explain  = shap.TreeExplainer(model)
strategy = LangChain.generate(shap_output)
```

![XGBoost](https://img.shields.io/badge/XGBoost-000?style=flat-square&logoColor=white)
![SHAP](https://img.shields.io/badge/SHAP-111?style=flat-square&logoColor=white)
![LangChain](https://img.shields.io/badge/LangChain-222?style=flat-square&logoColor=white)
![Streamlit](https://img.shields.io/badge/Streamlit-333?style=flat-square&logoColor=white)

</td>
<td width="4%" valign="top">
<br/><sub><code>02</code></sub>
</td>
<td width="46%" valign="top">

### Real-Time Jailbreak Detection
*AI Safety · Streaming · NLP*

**DistilBERT** classifier over **Apache Pulsar** with hot-swap model watcher. Adversarial prompt dataset inspired by JailbreakBench. Sub-100ms inference latency at scale.

```python
stream   = PulsarConsumer(topic="prompts")
model    = DistilBERT.load(hot_swap=True)
decision = model.classify(stream.next())
```

![DistilBERT](https://img.shields.io/badge/DistilBERT-000?style=flat-square)
![Pulsar](https://img.shields.io/badge/Apache%20Pulsar-111?style=flat-square)
![PyTorch](https://img.shields.io/badge/PyTorch-222?style=flat-square)
![HuggingFace](https://img.shields.io/badge/HuggingFace-333?style=flat-square)

</td>
</tr>
<tr><td colspan="4"><br/></td></tr>
<tr>
<td width="4%" valign="top">
<br/><sub><code>03</code></sub>
</td>
<td width="46%" valign="top">

### Credit Card Fraud · HDBSCAN
*Unsupervised Learning · Fraud Detection · XAI*

Cluster-based default prediction on **30k clients**. HDBSCAN segmentation → per-cluster Gradient Boosting → SMOTE oversampling → SHAP explainability. Production-ready Flask REST API.

```python
clusters = HDBSCAN().fit(X_30k)
models   = {c: GBM().fit(X[c]) for c in clusters}
explain  = SHAP.explain(models, X_test)
```

![HDBSCAN](https://img.shields.io/badge/HDBSCAN-000?style=flat-square)
![GBM](https://img.shields.io/badge/GradientBoosting-111?style=flat-square)
![SMOTE](https://img.shields.io/badge/SMOTE-222?style=flat-square)
![Flask](https://img.shields.io/badge/Flask-333?style=flat-square)

</td>
<td width="4%" valign="top">
<br/><sub><code>04</code></sub>
</td>
<td width="46%" valign="top">

### Smart Belt for Visually Impaired
*Embedded AI · IoT · Hardware*

Arduino + GPS + ultrasonic sensors for real-time obstacle detection and haptic feedback navigation. Edge AI meets assistive technology.

```c
while (true) {
  distance = ultrasonic.measure();
  if (distance < THRESHOLD)
    haptic.vibrate(intensity(distance));
}
```

![Arduino](https://img.shields.io/badge/Arduino-000?style=flat-square)
![IoT](https://img.shields.io/badge/IoT-111?style=flat-square)
![GPS](https://img.shields.io/badge/GPS-222?style=flat-square)
![Embedded](https://img.shields.io/badge/Embedded-333?style=flat-square)

</td>
</tr>
</table>

<br/>

---

<br/>

## Stack

<br/>

<table width="100%">
<tr>
<td width="25%" valign="top">

**AI · ML**

```
Python ············ ████████
PyTorch ··········· ███████░
TensorFlow ········ ██████░░
scikit-learn ······ ███████░
XGBoost ··········· ███████░
SHAP ·············· ██████░░
```

</td>
<td width="25%" valign="top">

**NLP · LLMs**

```
HuggingFace ······· ███████░
LangChain ········· ██████░░
DistilBERT ········ ██████░░
RAG Systems ······· █████░░░
Transformers ······ ██████░░
```

</td>
<td width="25%" valign="top">

**Data · Infra**

```
Apache Pulsar ····· █████░░░
Pandas · NumPy ···· ████████
MySQL ·············· ██████░░
Docker ············· ██████░░
Flask ·············· ███████░
Streamlit ·········· ███████░
```

</td>
<td width="25%" valign="top">

**Languages**

```
Python ············ ████████
Java ·············· █████░░░
SQL ··············· ██████░░
Bash ·············· █████░░░
```

</td>
</tr>
</table>

<br/>

---

<br/>

## Certifications

<br/>

<div align="center">

| Abbr | Certification | Issuer | Domain |
|:----:|:-------------|:------:|:------:|
| **CTM** | Cyber Threat Management | Cisco | Security |
| **NET** | Network Technician | Cisco | Networks |
| **IIoT** | Industrial IoT | UM6P | IoT |
| **OCI·AI** | Cloud Infrastructure AI | Oracle | Cloud |

</div>

<br/>

---

<br/>

## GitHub Activity

<br/>

<div align="center">

[![GitHub Streak](https://github-readme-streak-stats.herokuapp.com?user=ayayoussfiii&theme=dark&hide_border=true&background=0D0D0D&ring=ffffff&fire=ffffff&currStreakLabel=ffffff&sideLabels=666666&dates=666666&sideNums=ffffff&currStreakNum=ffffff&border=222222&stroke=222222)](https://github.com/ayayoussfiii)

</div>

<br/>

<div align="center">

[![GitHub Stats](https://github-readme-stats.vercel.app/api?username=ayayoussfiii&show_icons=true&hide_border=true&bg_color=0D0D0D&title_color=ffffff&icon_color=ffffff&text_color=666666&include_all_commits=true&count_private=true)](https://github.com/ayayoussfiii)&nbsp;&nbsp;[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=ayayoussfiii&layout=compact&hide_border=true&bg_color=0D0D0D&title_color=ffffff&text_color=666666&langs_count=6)](https://github.com/ayayoussfiii)

</div>

<br/>

<div align="center">

[![Activity Graph](https://github-readme-activity-graph.vercel.app/graph?username=ayayoussfiii&bg_color=0d0d0d&color=666666&line=ffffff&point=ffffff&area=true&area_color=222222&hide_border=true&custom_title=Contribution%20Graph)](https://github.com/ayayoussfiii)

</div>

<br/>

---

<br/>

<div align="center">

<sub><i>— "Build systems that explain themselves." —</i></sub>

<br/><br/>

![Visitors](https://komarev.com/ghpvc/?username=ayayoussfiii&color=ffffff&style=flat-square&label=profile+views)

<br/><br/>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0a0a0a,50:111111,100:0a0a0a&height=120&section=footer" width="100%"/>

</div>
