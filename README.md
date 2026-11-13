<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=rect&color=0:742774,100:0066FF&height=120&text=Cyber%20%E2%80%94%20IRP&fontSize=46&fontColor=ffffff&desc=Information%20Security%20Incident%20Management%20App&descAlignY=78&descSize=16&fontAlignY=42" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Power%20Apps-742774?style=for-the-badge&logo=powerapps&logoColor=white" />
  <img src="https://img.shields.io/badge/Power%20Automate-0066FF?style=for-the-badge&logo=powerautomate&logoColor=white" />
  <img src="https://img.shields.io/badge/PowerFX-555?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black" />
  <img src="https://img.shields.io/badge/Excel-217346?style=for-the-badge&logo=microsoftexcel&logoColor=white" />
  <br/>
  <img src="https://img.shields.io/badge/period-Dec%202023%20→%20Feb%202024-555?style=flat-square" />
  <img src="https://img.shields.io/badge/company-Votorantim%20Cimentos-555?style=flat-square" />
  <img src="https://img.shields.io/badge/method-Scrumban-555?style=flat-square" />
</p>

<p align="center"><img src="cover.jpg" width="85%" alt="Cyber IRP app" /></p>

## 🛡️ Overview

An application for **Information Security incident management** (IRP — Incident Response), built end-to-end on the **Microsoft Power Platform**.

## 🏗️ How it works

```mermaid
flowchart LR
    A[Power Automate<br/>ETL] --> B[(SharePoint List<br/>operational base)]
    B <--> C[Power Apps<br/>analyst interface]
    C -->|closed incidents| E[(Excel<br/>history)]
    E --> D[Power BI<br/>visualization]
```

| Layer | Technology | Role |
|---|---|---|
| ⚙️ Extraction & transformation | **Power Automate** (PowerFX) | Captures and prepares incident data |
| 🗄️ Storage | **SharePoint List** + **Excel** | Operational base + historical repository |
| 📱 Interface | **Power Apps** (PowerFX) | Where the team registers and manages incidents |
| 📊 Visualization | **Power BI** | Indicators — see [CyberSecurity Incidents Dashboard](https://github.com/MatheusFelipePereira/cybersecurity-incidents-dashboard) |

## 🔄 Incident lifecycle

1. **Power Automate** detects, extracts, transforms and loads (ETL) cybersecurity incidents into a **SharePoint List** — the operational base.
2. Analysts open the **Power Apps** app to validate each incident and complete it after analysis and response (e.g. *false positive*, *spam*, *real incident*).
3. The incident is **closed**, and consolidated data is stored in an **Excel** historical base.
4. That base feeds **Power BI** — stage two of the project: the [CyberSecurity Incidents Dashboard](https://github.com/MatheusFelipePereira/cybersecurity-incidents-dashboard).

## 🚀 Results

| | |
|---|---|
| ⏱️ **100+ hours** | of analysts' manual work eliminated |
| ⚡ **+30%** | team operational capacity for analysis, response and reporting to leadership |

## 📸 App gallery

<p align="center"><img src="img/01.png" width="320" /></p>

<table>
  <tr>
    <td width="50%" align="center"><img src="img/02.png" /><br/><sub><b>Welcome / loading screen</b></sub></td>
    <td width="50%" align="center"><img src="img/03.png" /><br/><sub><b>App screen</b></sub></td>
  </tr>
  <tr>
    <td width="50%" align="center"><img src="img/04.png" /><br/><sub><b>Register a new incident</b> in the queue</sub></td>
    <td width="50%" align="center"><img src="img/05.png" /><br/><sub><b>App screen</b></sub></td>
  </tr>
  <tr>
    <td width="50%" align="center"><img src="img/06.png" /><br/><sub><b>App screen</b></sub></td>
    <td width="50%" align="center"><img src="cover.jpg" /><br/><sub><b>Power BI output</b></sub></td>
  </tr>
</table>

## 👥 Team

Built with César at **Votorantim Cimentos**, in a **Scrumban** flow.

---

<sub>🔒 Corporate project: incident data is confidential, so this repository documents the solution only.  
👤 Part of <a href="https://github.com/MatheusFelipePereira">Matheus Felipe Pereira's portfolio</a> · <a href="https://www.linkedin.com/in/matheus-felipe-p/">LinkedIn</a></sub>
