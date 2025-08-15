# 🚀 MCP Comprehensive AI Agent

A **Google ADK-based AI Agent** powered by `gemini-2.0-flash` that connects to **ServiceNow** via the **Model-Callable Proxy (MCP)** toolset.  
This agent supports **searching, creating, updating, and retrieving** any ServiceNow record type using **natural language**—no ServiceNow query syntax required.

---

## ✨ Features

- **🔍 Search & Find (Any Record Type)**
  - Example:  
    - `Find all incidents`  
    - `Show high priority incidents`  
    - `Search for users in IT department`
  - Supports **incidents**, **change requests**, **problems**, **users**, **groups**, **CMDB**, **knowledge articles**, **service catalog items**, and more.

- **➕ Create Records**
  - Example:  
    - `Create incident for email server down`  
    - `Create change request for server upgrade`

- **✏️ Update & Modify Records**
  - Example:  
    - `Update incident INC0010001 to in progress`  
    - `Add comment to INC0010001: Contacted user`  
    - `Add work note to INC0010001: Checked server logs`

- **📋 Retrieve & Display Details**
  - Example:  
    - `Get incident INC0010001`  
    - `Show change request CHG0012345`

---

## 🗂 Project Structure

```plaintext
.
├── main.py                  # Main agent definition & MCP toolset connection
├── .env                     # Environment variables for ServiceNow credentials
├── requirements.txt         # Python dependencies
└── README.md                # Documentation

-##1️⃣ Clone the Repository
git clone https://github.com/yourusername/servicenow-mcp-agent.git
cd servicenow-mcp-agent

##2️⃣ Create and Activate a Virtual Environment
python -m venv venv
source venv/bin/activate   # Mac/Linux
venv\Scripts\activate      # Windows

##3️⃣ Install Python Dependencies
pip install -r requirements.txt

##4️⃣ Set Up Environment Variables
SERVICENOW_INSTANCE_URL=https://your-instance.service-now.com
SERVICENOW_USERNAME=your-username
SERVICENOW_PASSWORD=your-password

▶️ Running the Agent
adk web
