<h1 align="center">
  <br/>
  Aya Youssfi
  <br/>
</h1>

<p align="center">
  <code>AI & Digital Trust Engineering</code> &nbsp;·&nbsp; <code>ENSA Fès, Morocco</code>
</p>

<p align="center">
  <a href="https://linkedin.com/in/aya-youssfi">
    <img src="https://img.shields.io/badge/LinkedIn-aya--youssfi-0A66C2?style=flat-square&logo=linkedin&logoColor=white"/>
  </a>
  &nbsp;
  <a href="mailto:aya.youssfi@usmba.ac.ma">
    <img src="https://img.shields.io/badge/Email-aya.youssfi%40usmba.ac.ma-EA4335?style=flat-square&logo=gmail&logoColor=white"/>
  </a>
  &nbsp;
  <a href="https://github.com/ayayoussfiii">
    <img src="https://img.shields.io/badge/GitHub-ayayoussfiii-181717?style=flat-square&logo=github&logoColor=white"/>
  </a>
  &nbsp;
  <img src="https://img.shields.io/badge/Status-Open%20to%20Internships-2ea44f?style=flat-square"/>
</p>

<br/>

```python
class AyaYoussfi:
    school   = "ENSA Fès — Cycle Ingénieur · AI & Digital Trust"
    focus    = ["Explainable AI", "RAG Systems", "AI Safety", "Real-Time ML"]
    stack    = ["Python", "PyTorch", "LangChain", "HuggingFace", "Docker", "SHAP"]
    looking  = ["Internship", "Research Collaboration", "Open Source"]
    motto    = "Build systems that explain themselves."
```

<br/>

---

## 01 · Projects

<br/>

<table>
<tr>
<td valign="top" width="50%">

**🧠 Customer Churn + LLM Retention**
`Machine Learning · XAI · NLP`

End-to-end pipeline · XGBoost classifier · SHAP explainability · LLM-generated personalised retention strategies · Streamlit dashboard.

```python
model    = XGBoostClassifier().fit(X_train)
explain  = shap.TreeExplainer(model)
strategy = llm.generate(explain.values)
```

![](https://img.shields.io/badge/XGBoost-189ABF?style=flat-square)
![](https://img.shields.io/badge/SHAP-343434?style=flat-square)
![](https://img.shields.io/badge/LangChain-1C3C3C?style=flat-square&logoColor=white)
![](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square)

</td>
<td valign="top" width="50%">

**🛡️ Real-Time Jailbreak Detection**
`AI Safety · Streaming · NLP`

DistilBERT classifier over Apache Pulsar · Hot-swap model watcher · Adversarial prompts · Sub-100ms latency.

```python
stream   = PulsarConsumer(topic="prompts")
model    = AutoModel.load(hot_swap=True)
label    = model.classify(stream.next())
```

![](https://img.shields.io/badge/DistilBERT-FFD21E?style=flat-square&logoColor=black)
![](https://img.shields.io/badge/Apache%20Pulsar-188FFF?style=flat-square)
![](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square)
![](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logoColor=black)

</td>
</tr>
<tr>
<td valign="top" width="50%">

**💳 Credit Card Fraud · HDBSCAN**
`Unsupervised Learning · Fraud Detection · XAI`

30k clients · HDBSCAN segmentation → per-cluster GBM → SMOTE → SHAP · Flask REST API.

```python
clusters = HDBSCAN().fit_predict(X)
models   = {c: GBM().fit(X[c]) for c in clusters}
api      = Flask(__name__).expose(models)
```

![](https://img.shields.io/badge/HDBSCAN-7C3AED?style=flat-square)
![](https://img.shields.io/badge/GBM-F59E0B?style=flat-square&logoColor=black)
![](https://img.shields.io/badge/SMOTE-10B981?style=flat-square)
![](https://img.shields.io/badge/Flask-000000?style=flat-square)

</td>
<td valign="top" width="50%">

**🦯 Smart Belt for Visually Impaired**
`Embedded AI · IoT · Hardware`

Arduino + GPS + ultrasonic sensors · Real-time obstacle detection · Haptic feedback navigation.

```c
while (true) {
  d = ultrasonic.read();
  if (d < THRESHOLD)
    haptic.pulse(map(d, 0, MAX, 255, 0));
}
```

![](https://img.shields.io/badge/Arduino-00979D?style=flat-square)
![](https://img.shields.io/badge/IoT-0EA5E9?style=flat-square)
![](https://img.shields.io/badge/GPS-374151?style=flat-square)
![](https://img.shields.io/badge/Embedded-4B5563?style=flat-square)

</td>
</tr>
</table>

<br/>

---

## 02 · Stack

<br/>

<table>
<tr>
<td valign="top" width="25%">

**AI · ML**
```
Python        ████████
PyTorch       ███████░
TensorFlow    ██████░░
scikit-learn  ███████░
XGBoost       ███████░
SHAP          ██████░░
```

</td>
<td valign="top" width="25%">

**NLP · LLMs**
```
HuggingFace   ███████░
LangChain     ██████░░
DistilBERT    ██████░░
RAG Systems   █████░░░
Transformers  ██████░░
```

</td>
<td valign="top" width="25%">

**Data · Infra**
```
Pandas/NumPy  ████████
Apache Pulsar █████░░░
MySQL         ██████░░
Docker        ██████░░
Flask         ███████░
Streamlit     ███████░
```

</td>
<td valign="top" width="25%">

**Languages**
```
Python        ████████
Java          █████░░░
SQL           ██████░░
Bash          █████░░░
```

</td>
</tr>
</table>

<br/>

---

## 03 · Certifications

<br/>

<table>
<tr>
<td align="center" width="25%">
  <img src="https://img.shields.io/badge/Cisco-1BA0D7?style=for-the-badge&logo=cisco&logoColor=white"/><br/>
  <sub><b>Cyber Threat Management</b></sub>
</td>
<td align="center" width="25%">
  <img src="https://img.shields.io/badge/Cisco-1BA0D7?style=for-the-badge&logo=cisco&logoColor=white"/><br/>
  <sub><b>Network Technician</b></sub>
</td>
<td align="center" width="25%">
  <img src="https://img.shields.io/badge/UM6P-00A651?style=for-the-badge&logoColor=white"/><br/>
  <sub><b>Industrial IoT</b></sub>
</td>
<td align="center" width="25%">
  <img src="https://img.shields.io/badge/Oracle-F80000?style=for-the-badge&logo=oracle&logoColor=white"/><br/>
  <sub><b>Cloud Infrastructure AI</b></sub>
</td>
</tr>
</table>

<br/>

---

## 04 · GitHub Activity

<br/>

<div align="center">

[![GitHub Streak](https://streak-stats.demolab.com?user=ayayoussfiii&theme=dark&hide_border=true&background=0D1117&ring=58a6ff&fire=58a6ff&currStreakLabel=58a6ff&sideLabels=8b949e&dates=8b949e&sideNums=e6edf3&currStreakNum=e6edf3)](https://github.com/ayayoussfiii)

</div>

<div align="center">

[![GitHub Stats](https://github-readme-stats.vercel.app/api?username=ayayoussfiii&show_icons=true&hide_border=true&bg_color=0D1117&title_color=58a6ff&icon_color=58a6ff&text_color=8b949e&include_all_commits=true&count_private=true)](https://github.com/ayayoussfiii)
&nbsp;
[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=ayayoussfiii&layout=compact&hide_border=true&bg_color=0D1117&title_color=58a6ff&text_color=8b949e&langs_count=6)](https://github.com/ayayoussfiii)

</div>

<br/>

---

<br/>

<p align="center">
  <sub><i>"Build systems that explain themselves."</i></sub>
  <br/><br/>
  <img src="https://komarev.com/ghpvc/?username=ayayoussfiii&color=58a6ff&style=flat-square&label=profile+views"/>
</p>
