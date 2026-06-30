# Recruitment Intelligence Agent 🧠

**Agentic Business Orchestration for Automated Recruitment**

Recruitment Intelligence Agent is a fully autonomous, production-ready UiPath BPMN workflow designed to revolutionize the recruitment pipeline. By leveraging **Agentic Business Orchestration**, this project eliminates manual HR screening and provides intelligent, data-driven candidate evaluations.

---

## 👥 Contributors

- **Asmit Samal** - [@Asmit1211](https://github.com/Asmit1211)
- **Vedant Vare** - [@VedantVare](https://github.com/VedantVare)
- **Parth More** - [@parthmore0707-alt](https://github.com/parthmore0707-alt)

---

## 🚀 Project Links

- **Demo Video:** [[ YOUTUBE LINK ](https://youtu.be/WfA45qVhvWM)]
- **Presentation (PPT):** [[ GOOGLE SLIDES LINK ](https://docs.google.com/presentation/d/1OG_-Nc_65V1lUxUd-E8AFAo8mUp7QuWL/edit?usp=sharing&ouid=106029780792893337727&rtpof=true&sd=true)]


---

## 🤖 The Agentic Flow

This workflow utilizes UiPath Maestro BPMN to create a sequential, multi-agent pipeline. It natively accepts dynamic inputs (`jobPosition`, `jobDescription`, and `pdf` file) via UiPath Orchestrator Start Event arguments.

---

## 📋 Workflow Pipeline

### 1. **Resume Parsing Agent**
Extracts unstructured PDF content into structured JSON format, capturing:
- Skills
- Education
- Experience

### 2. **Recruitment Intelligence Agent** (Powered by GPT-5.4)
The core decision-maker of the pipeline that:
- Cross-references the candidate profile against the job description
- Provides a precise fitment score
- Delivers detailed reasoning for the evaluation

### 3. **Candidate Communication Agent**
Finalizes the AI evaluation by:
- Structuring the assessment into organized logs
- Preparing the output for HR review
- Enabling automated feedback generation

---

## ⚙️ How to Run (Instructions for Judges)

### Step 1: Deploy
Import the `.nupkg` package into your UiPath Automation Cloud Orchestrator.

### Step 2: Trigger
Select **Start Job** on the published process in Orchestrator.

### Step 3: Provide Input
In the **Arguments** tab, provide the following parameters:

| Argument | Type | Description | Example |
|----------|------|-------------|---------|
| `jp` | String | Job Position | "AI Engineer" |
| `jd` | String | Full Job Description | "We are looking for..." |
| `pdf` | File | Candidate's Resume (PDF) | resume.pdf |

### Step 4: Monitor
Open **Process Logs** to view the real-time reasoning and decision-making of the sequential agents as they evaluate the candidate.

---

## 📁 Project Structure

```
Solution.uipx/
├── Agent/                              # Main orchestration agent
│   ├── agent.json
│   ├── entry-points.json
│   ├── flow-layout.json
│   ├── project.uiproj
│   └── evals/
├── Candidate Communication Agent/      # Final communication agent
│   ├── agent.json
│   ├── entry-points.json
│   ├── flow-layout.json
│   ├── project.uiproj
│   └── evals/
├── Maestro BPMN/                       # Core orchestration process
│   ├── Process.bpmn
│   ├── bindings_v2.json
│   ├── entry-points.json
│   └── project.uiproj
├── Recruitment Intelligence Agent/     # Intelligent evaluation agent
│   ├── agent.json
│   ├── entry-points.json
│   ├── flow-layout.json
│   ├── project.uiproj
│   └── evals/
├── Resume Parser Agent New/            # Resume extraction agent
│   ├── agent.json
│   ├── entry-points.json
│   ├── flow-layout.json
│   ├── project.uiproj
│   └── evals/
├── RPA Workflow/                       # Supporting RPA processes
│   ├── Main.xaml
│   ├── entry-points.json
│   ├── project.json
│   └── project.uiproj
└── resources/                          # Configuration and connections
    └── solution_folder/
        ├── connection/
        ├── package/
        └── process/
```

---

## 🛠️ Technologies & Tools

- **UiPath Maestro BPMN** - Workflow orchestration and process automation
- **UiPath Agents** - Agentic business orchestration
- **OpenAI GPT-5.4** - Intelligent candidate evaluation
- **UiPath Orchestrator** - Job execution and monitoring
- **PDF Processing** - Resume parsing and extraction

---

## 📊 Key Features

✅ **Fully Autonomous Pipeline** - End-to-end recruitment evaluation without manual intervention  
✅ **Data-Driven Insights** - Structured candidate assessments with scoring  
✅ **Multi-Agent Architecture** - Specialized agents for parsing, evaluation, and communication  
✅ **Production-Ready** - Tested and optimized for enterprise deployment  
✅ **Real-Time Monitoring** - Process logs provide transparency into agent reasoning  
✅ **Dynamic Inputs** - Flexible job descriptions and resume formats  

---

## 🎯 Use Cases

- **Automated Resume Screening** - Quickly filter candidates based on job requirements
- **Skill Matching** - Intelligently match candidate skills to job position requirements
- **Candidate Ranking** - Generate comparable fitment scores across applicants
- **HR Automation** - Reduce manual HR review time by up to 80%
- **Recruitment Analytics** - Gain insights into candidate pools and hiring patterns

---

## 📝 Notes for Judges

- **Track:** UiPath AgentHack 2026 - Track 2 (UiPath Maestro BPMN)
- **Deployment:** The solution is packaged as a `.nupkg` file for direct deployment
- **Scalability:** Designed to handle high-volume recruitment pipelines
- **Customization:** Job descriptions and evaluation criteria can be easily modified

---

## 📧 Support & Contact

For questions or issues, please reach out to:
- Asmit Samal ([@Asmit1211](https://github.com/Asmit1211))

---

**Built for UiPath AgentHack 2026 | Track 2 - UiPath Maestro BPMN**

