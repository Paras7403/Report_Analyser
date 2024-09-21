# Blood Test Analysis Workflow
This Jupyter Notebook automates the process of analyzing blood test reports and providing health recommendations based on the findings. It utilizes CrewAI, a library for task automation and delegation, along with PyPDF2 for reading PDF files and some additional tools for searching the web.

# Approach:
Reading Blood Test Reports: The notebook extracts text from specific pages of a PDF blood test report using PyPDF2.

Agent and Task Definition: We define three types of agents - Blood Test Analyst, Article Researcher, and Health Advisor. Each agent has a specific role in the workflow. Tasks are also defined, each assigned to a specific agent.

Executing Tasks: The Crew is formed with agents and tasks. Each task is executed sequentially, passing context from one task to another.

# Steps to Run the Code:
1) Install Required Packages: Make sure you have Python installed on your system. Install the required packages using pip:

CODE:- 
pip install crewai PyPDF2

2) Set Up API Keys: Before running the notebook, replace the empty strings with your API keys. Update the following lines with your Serper API key and OpenAI API key:

os.environ["SERPER_API_KEY"] = "<your_serper_api_key>"
os.environ["OPENAI_API_KEY"] = "<your_openai_api_key>"

3) Download PDF Blood Test Report: Download the PDF blood test report that you want to analyze and update the pdf variable in the notebook with the correct file path.

4) Run the Notebook: Execute the Jupyter Notebook. You can run each cell one by one or all at once, depending on your preference.

5) Review Output: Once the notebook completes execution, review the output. You should see the summary of blood test results and health recommendations based on the articles found.
