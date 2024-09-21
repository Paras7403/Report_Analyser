# Blood Test Analysis Workflow

This Jupyter Notebook automates the analysis of blood test reports and provides health recommendations based on the findings. The workflow leverages **CrewAI** for task automation, **PyPDF2** for reading PDF files, and additional tools for web research.

## Features

- **Blood Test Report Reading**: Extracts data from specific pages of a PDF blood test report.
- **Automated Task Assignment**: Uses various agents (Blood Test Analyst, Article Researcher, Health Advisor) to analyze, research, and provide health recommendations.
- **Seamless Workflow Execution**: Tasks are executed sequentially, passing context from one to another for efficient processing.

---

## Prerequisites

Before running the notebook, ensure that you have the following requirements:

### 1. Install Required Packages

Ensure Python is installed, and then install the required libraries by running the following command:

```bash
pip install crewai PyPDF2
```

### 2. Set Up API Keys

The workflow requires API keys for certain tasks. Set up your environment by replacing the placeholders with your actual keys.

```bash
os.environ["SERPER_API_KEY"] = "<your_serper_api_key>"
os.environ["OPENAI_API_KEY"] = "<your_openai_api_key>"
```

### 3.  Download PDF Blood Test Report

Download the PDF blood test report you want to analyze and update the file path in the notebook.

```bash
pdf = "<path_to_your_blood_test_report.pdf>"
```

---

# Running the Workflow
- **Open the Jupyter Notebook** : Open the Jupyter Notebook containing the workflow.
- **Execute the Cells** : Run the cells in the notebook sequentially, or execute all at once depending on your preference.
- **Review the Output** : Upon execution, you'll receive a summary of blood test results and personalized health recommendations based on web research.

---

# Workflow Agents
- **Blood Test Analyst** : Extracts and analyzes the blood test results.
- **Article Researcher** : Searches for articles related to any abnormal findings or relevant health metrics.
- **Health Advisor** : Provides health recommendations based on the research and analysis.

---

# Notes
- Ensure your PDF blood test report is formatted properly for text extraction.
- The health recommendations are based on automated web research and always consult a healthcare professional for medical advice.

