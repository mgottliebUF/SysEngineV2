# SysEngineV2
This is a systems engineering toolkit that will allow systems engineers to be more effective. 

To run this project, open an IDE (example: Jupyter notebook) and copy/paste the script. 

You can save a copy of your project and after re-running the script, you can open a saved JSON of your project and continue to build your product. 

This is the public version of the script and an additonal SysML modeling feature and LLM feature are being integrated into a private version of the product. 

The ultimate goal is to integrate the Engineering LLM model in development to provide requirement traceability suggestions and use an additonal seperate model to create SysML viewpoints automatically based on requirements and CONOPS information. 

MBSE Tool
A Model-Based Systems Engineering (MBSE) desktop application built with Python and PyQt5. This tool provides a graphical environment for managing requirements, system decomposition, tests, actions, and conceptual information related to systems engineering projects. It integrates various aspects such as requirements handling, test verification tracking, system state progression, and even includes placeholders for CAD models and JIRA integration.

Table of Contents
Features
Screenshots
Installation
Prerequisites
Setup Steps
Usage
Running the Application
Creating a New Project
Loading an Existing Project
Saving a Project
Core Components
Home Page
Requirements Manager
System State Tracker
CONOPS
System Decomposition
Action Manager
Test Verification
CAD Models
JIRA Integration (Placeholder)
Glossary
Reliability Tools
Data Persistence
Development Notes
Contributing
License
Features
Requirements Management:
Create, edit, import, and export requirements. Apply filters, bulk-edit multiple requirements, and view them in a tree or table format.

System Decomposition:
Define decompositions of your system (e.g., System, Subsystem, Component) and edit their details.

Test Verification:
Link tests to requirements, track test status, method, date, and results. Add, edit, or remove tests.

Action Management:
Keep track of system actions, their descriptions, and statuses.

System State Tracking:
Manage the system engineering lifecycle stage (e.g., Concept Development, Requirements Analysis, etc.).

CONOPS:
Capture the concept of operations including purpose, scope, operational context, stakeholders, scenarios, capabilities, constraints, risks, and metrics for success.

Glossary Management:
Maintain a subsystem glossary (terminology and definitions) to keep everyone aligned.

Reliability Tools:
Simple reliability calculations (e.g., MTBF) based on input failure rates.

Project Data Tree View (Containment Tree):
Quickly navigate between requirements, tests, actions, decompositions, and glossary terms from a dockable containment tree.

Import/Export:
Requirements and Projects can be loaded from and saved to JSON and CSV files.

Placeholder Integrations:
CAD Models tab and JIRA Integration tab are currently placeholders for future feature expansions.

Screenshots
(Include relevant screenshots of the UI if available.)

Installation
Prerequisites
Python 3.7 or higher
PyQt5 for GUI components
(Optional) Additional packages as needed for advanced features
Setup Steps
Clone the repository:

bash
Copy code
git clone https://github.com/your-username/mbse-tool.git
cd mbse-tool
Install dependencies:

bash
Copy code
pip install -r requirements.txt
(If requirements.txt is not provided, simply run pip install pyqt5.)

Usage
Running the Application
From the project directory, run:

bash
Copy code
python your_script_name.py
(Replace your_script_name.py with the actual filename if you rename it.)

This will launch the MBSE tool GUI application.

Creating a New Project:
Click "New Project" on the top toolbar.
Choose a location and name for your JSON project file.
Once created, you'll have a blank slate to start adding requirements, tests, and other data.

Loading an Existing Project:
Click "Open Project" on the toolbar.
Select the previously saved .json project file.
The application will load all previously saved data (requirements, tests, decompositions, etc.).

Saving a Project:
Click "Save Project" on the toolbar.
Choose a location and name for the JSON file.
All current data within the tabs (requirements, tests, CONOPS, decomposition, etc.) will be saved for future reuse.

Home Page:
The landing page with a title and brief application description. No data editing here, just a welcome interface.

Requirements Manager:
View Modes: Switch between a tree view and a table view of requirements.
Filtering: Filter requirements by category, archived state, or a search keyword.
Bulk Edit: Select multiple requirements and apply priority or status changes at once.
CSV Import/Export: Import requirements from a CSV file or export them for documentation.
System State Tracker

Lifecycle Stage: Choose from different stages (e.g., Concept Development, Requirements Analysis) to reflect where the project stands in the engineering process.

Toolbar Sync: The selected system state is displayed on the toolbar.

CONOPS:
Capture high-level operational concepts, including scope, stakeholders, operational scenarios, constraints, and more.
System Decomposition
Define hierarchical system elements (e.g., System > Subsystem > Component).
Add, edit, or delete entries to reflect the evolving architecture of your system.

Action Manager:
Track actions needed for the project (e.g., tasks, issues).
Add new actions, delete them, and keep an overview of what’s pending.

Test Verification:
Link tests directly to requirements.
Track verification methods, statuses, results, and test dates.
Add/edit/delete tests as the project progresses.

CAD Models:
A placeholder section to visualize or link CAD models. Currently displays a placeholder message.
Future integration might load and display .stl or other 3D model formats.

JIRA Integration (Placeholder):
Demonstrates where JIRA or other issue tracking integrations could occur.
Currently aesthetic only, no real JIRA functionality implemented.

Glossary:
Maintain a glossary of subsystem terms and definitions.
Add new terms and definitions or edit existing ones.
Useful for ensuring consistent terminology across the project.

Reliability Tools:
Enter a component failure rate and compute Mean Time Between Failures (MTBF).
View best practices for improving system reliability.

Data Persistence:
Projects: Stored in a JSON file containing requirements, tests, actions, decomposition data, system state, and CONOPS.

Requirements: Can be imported/exported separately via CSV for easy integration with external tools.

Development Notes:
UI Framework: Uses PyQt5 for cross-platform desktop GUI.
Code Structure: The code organizes different functional sections as separate classes/widgets. The main window (MBSETool class) manages tabs, toolbars, and data loading/saving.
Extensibility: Designed to be expandable. Additional functionality (e.g., DODAF views, custom integrations) can be added by creating new widgets and extending the main application.
![image](https://github.com/user-attachments/assets/95ada4fb-5e99-43a0-82ad-0344d8c17e2f)


