<h1 align="center">Aya Youssfi</h1>

<p align="center">
  <code>AI & Digital Trust Engineering</code> &nbsp;·&nbsp; <code>ENSA Fès, Morocco</code>
</p>

<p align="center">
  <a href="https://linkedin.com/in/aya-youssfi">
    <img src="https://img.shields.io/badge/LinkedIn-aya--youssfi-0A66C2?style=flat-square&logo=linkedin&logoColor=white"/>
  </a>&nbsp;
  <a href="mailto:aya.youssfi@usmba.ac.ma">
    <img src="https://img.shields.io/badge/Email-aya.youssfi%40usmba.ac.ma-EA4335?style=flat-square&logo=gmail&logoColor=white"/>
  </a>&nbsp;
  <a href="https://github.com/ayayoussfiii">
    <img src="https://img.shields.io/badge/GitHub-ayayoussfiii-181717?style=flat-square&logo=github&logoColor=white"/>
  </a>&nbsp;
  <img src="https://img.shields.io/badge/Status-Open%20to%20Internships-2ea44f?style=flat-square"/>&nbsp;
  <img src="https://komarev.com/ghpvc/?username=ayayoussfiii&color=5b8dee&style=flat-square&label=profile+views"/>
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

## `01` &nbsp; Projects

<br/>

<table>
<tr>
<td valign="top" width="50%">

![](https://img.shields.io/badge/Machine%20Learning%20·%20XAI-e8a838?style=flat-square&logoColor=black)

**🧠 Customer Churn + LLM Retention**

End-to-end pipeline · XGBoost classifier · SHAP explainability · LLM-generated personalised retention strategies · Streamlit dashboard.

```python
model    = XGBoostClassifier().fit(X_train)
explain  = shap.TreeExplainer(model)
strategy = llm.generate(explain.values)
```

![](https://img.shields.io/badge/XGBoost-e8a838?style=flat-square&logoColor=black)
![](https://img.shields.io/badge/SHAP-d4922a?style=flat-square&logoColor=white)
![](https://img.shields.io/badge/LangChain-5b8dee?style=flat-square&logoColor=white)
![](https://img.shields.io/badge/Streamlit-FF4B4B?style=flat-square&logoColor=white)

</td>
<td valign="top" width="50%">

![](https://img.shields.io/badge/AI%20Safety%20·%20Streaming-e85555?style=flat-square&logoColor=white)

**🛡️ Real-Time Jailbreak Detection**

DistilBERT classifier over Apache Pulsar · Hot-swap model watcher · Adversarial prompts · Sub-100ms latency.

```python
stream = PulsarConsumer(topic="prompts")
model  = AutoModel.load(hot_swap=True)
label  = model.classify(stream.next())
```

![](https://img.shields.io/badge/DistilBERT-e85555?style=flat-square&logoColor=white)
![](https://img.shields.io/badge/Apache%20Pulsar-c43e3e?style=flat-square&logoColor=white)
![](https://img.shields.io/badge/PyTorch-EE4C2C?style=flat-square&logoColor=white)
![](https://img.shields.io/badge/HuggingFace-FFD21E?style=flat-square&logoColor=black)

</td>
</tr>
<tr>
<td valign="top" width="50%">

![](https://img.shields.io/badge/Fraud%20Detection%20·%20XAI-a855f7?style=flat-square&logoColor=white)

**💳 Credit Card Fraud · HDBSCAN**

30k clients · HDBSCAN segmentation → per-cluster GBM → SMOTE oversampling → SHAP · Flask REST API.

```python
clusters = HDBSCAN().fit_predict(X)
models   = {c: GBM().fit(X[c]) for c in clusters}
api      = Flask(__name__).expose(models)
```

![](https://img.shields.io/badge/HDBSCAN-a855f7?style=flat-square&logoColor=white)
![](https://img.shields.io/badge/GBM-8b3fd4?style=flat-square&logoColor=white)
![](https://img.shields.io/badge/SMOTE-7c35bb?style=flat-square&logoColor=white)
![](https://img.shields.io/badge/Flask-000000?style=flat-square&logoColor=white)

</td>
<td valign="top" width="50%">

![](https://img.shields.io/badge/Embedded%20AI%20·%20IoT-2ea44f?style=flat-square&logoColor=white)

**🦯 Smart Belt for Visually Impaired**

Arduino + GPS + ultrasonic sensors · Real-time obstacle detection · Haptic feedback navigation at the edge.

```c
while (true) {
  d = ultrasonic.read();
  if (d < THRESHOLD)
    haptic.pulse(map(d, 0, MAX, 255, 0));
}
```

![](https://img.shields.io/badge/Arduino-00979D?style=flat-square&logoColor=white)
![](https://img.shields.io/badge/IoT-2ea44f?style=flat-square&logoColor=white)
![](https://img.shields.io/badge/GPS-1a7a38?style=flat-square&logoColor=white)
![](https://img.shields.io/badge/Embedded-145c2a?style=flat-square&logoColor=white)

</td>
</tr>
</table>

<br/>

---

## `02` &nbsp; Stack

<br/>

<table>
<tr>
<td valign="top" width="25%">

**🔵 AI · ML**
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

**🟡 NLP · LLMs**
```
HuggingFace   ███████░
LangChain     ██████░░
DistilBERT    ██████░░
RAG Systems   █████░░░
Transformers  ██████░░
```

</td>
<td valign="top" width="25%">

**🟢 Data · Infra**
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

**🔴 Languages**
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

## `03` &nbsp; Certifications

<br/>

<table>
<tr>
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
<td align="center" width="25%">
  <img src="https://img.shields.io/badge/OCI·AI-F80000?style=for-the-badge&logo=oracle&logoColor=white"/><br/><br/>
  <sub><b>Cloud Infrastructure AI</b></sub><br/>
  <sub>Oracle</sub>
</td>
</tr>
</table>

<br/>

---

## `04` &nbsp; GitHub Activity

<br/>

<p align="center">
  <img src="https://img.shields.io/badge/Contributions-298-5b8dee?style=for-the-badge&logoColor=white"/>
  &nbsp;
  <img src="https://img.shields.io/badge/Current%20Streak-4%20days-2ea44f?style=for-the-badge&logoColor=white"/>
  &nbsp;
  <img src="https://img.shields.io/badge/Longest%20Streak-6%20days-e8a838?style=for-the-badge&logoColor=black"/>
  &nbsp;
  <img src="https://img.shields.io/badge/Since-Nov%202025-e85555?style=for-the-badge&logoColor=white"/>
</p>

<br/>

```
  Contribution graph — Nov 2025 → Jun 2026

  Nov  ░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░░
  Dec  ░░▒▒░░░░░▒▒▒░░░░░░░▒░░░░░░▒▒░░
  Jan  ░▒▒░░░▒▒▒▒░░░░▒▒░░░░░▒▒▒░░░░░░
  Feb  ░░░░▒▒░░░░░░▒▒▒▒░░░▒░░░░▒▒▒░░░
  Mar  ▒▒░░░░░░▒▒▒░░░░░▒▒░░░░▒▒░░░░▒▒
  Apr  ░░▒▒▒░░░░░░▒▒░░░▒▒▒▒▒▒▒░░░░░░░
  May  ░░░░▒▒▒░░░░░▒▒▒░░░░░▒▒▒▒▒▒▒▒▒▒
                                  ↑ now
  ░ no activity   ▒ active   298 total contributions
```

<br/>

---

<br/>

<p align="center">
  <i>"Build systems that explain themselves."</i>
</p>

<br/>
