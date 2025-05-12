# Crew AI
# INSTALLATION PROCESS:
# 1.1] Python Version Requirements:
python3 –version [Python 3.11.9]
# 1.2] UV 
CrewAI uses the uv as its dependency management and package handling tool.
On Windows:
Use irm to download the script and iex to execute it:
powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
-Extract and place the uv.exe folder path to your system PATH.
# 1.3] Install CrewAI:
uv --version [uv 0.7.3]
uv venv .venv
uv pip install crewai  
Note: If you encounter a PATH warning, run this command to update your shell: 
uv tool update-shell 
# 1.4] To verify that crewai is installed 
venv> uv tool list
crewai v0.118.0
- crewai.exe
-If you need to update crewai, run: uv tool install crewai –upgrade
# Creating a CrewAI Project
# 2.1] Generate Project Scaffolding
crewai create crew <folder_name>
[select based on your requirement]
Select a provider to set up: ollama
Select a model to use for Ollama:
Selected model: ollama/llama3.1
Crew madhu_crewai created successfully!
Customize Your Project
our project will contain these essential files:
File	Purpose
aents.yaml	AI agents and their roles [Role, goal, backstory]
tasks.yaml	Set up agent tasks and workflows [task, description, agent]
.env	It stores API keys and environment variables [Model, API Base]
main.py	Project entry point and execution flow [any input]
crew.py	Crew orchestration and coordination [agent, task, crew]

# 2.2] Navigate to your new crew project < madhu_crewai>
Go to your folder < madhu_crewai >  
And change agents. yaml, tasks. yaml, main.py, crew.py, .env,
then run
crewai install
# 2.3] Set your environment variables
OPENAI_API_KEY= <YOUR_API_KEY>
SERPER_API_KEY=<YOUR_SERPER_KEY>

# 2.4] Install the dependencies
- crewai install
# 2.5] Run your crew
-crewai run

