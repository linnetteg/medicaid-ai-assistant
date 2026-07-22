# Medicaid AI Assistant

### AI-Powered Healthcare Workflow Automation

The **Medicaid AI Assistant** is a production Python application that automates weekly Medicaid case management documentation for long-term care residents.

By combining **OpenAI**, **Python**, and **Microsoft Excel automation**, the application transforms internal case notes into professional weekly Medicaid summaries while preserving case continuity, unresolved issues, and historical documentation.

This application is actively used in production to automate weekly Medicaid case documentation and continues to evolve into a broader healthcare workflow automation platform.

Originally developed to solve a real operational challenge, it reduces repetitive documentation from **several hours each week to under one minute**, allowing more time to focus on resident advocacy, case management, and complex eligibility work rather than repetitive data entry.

This project demonstrates practical applications of Python, OpenAI, prompt engineering, workflow automation, and Excel integration in a real-world healthcare operations environment. The application is designed around modular architecture, separating AI prompting, Excel management, reporting logic, and workflow utilities into independent components for long-term scalability.

---

## Why I Built This

As a Medicaid Eligibility Specialist, I noticed I was spending hours each week rewriting nearly identical case updates while trying to maintain continuity across hundreds of active residents.

Rather than accepting the process, I designed and built an AI-assisted workflow that automates the repetitive documentation while preserving the accuracy and professional standards required for Medicaid case management.

This project is actively used in a real production workflow and continues to evolve with new automation features.

---

# Current Version

**v2.1**

## Project Status

🚧 Actively Under Development

---

# Features

- 🤖 AI-generated weekly Medicaid case summaries
- 📋 Intelligent carry-forward of unresolved case activity
- ⏭ Automatically skips residents already updated for the current reporting period
- 📊 Resident progress tracking during execution
- 💾 Automatic timestamped workbook backups
- 📝 Run logging
- 📎 Preserves:
  - Microsoft 365 checkboxes
  - Hyperlinks
  - Cell formatting
  - Tables
  - Filters
- ⚡ Built using **xlwings** to preserve modern Excel functionality

---

# Current Workflow

```text
                    MedicaidTracker.xlsx

                            │

                Previous Weekly Update
                            │
                Current Case Notes
                            │
                            ▼
                 Medicaid AI Assistant
                            │
        ┌───────────────────┼──────────────────┐
        │                   │                  │
        ▼                   ▼                  ▼
 Automatic Backup     AI Weekly Update     Run Log
        │                   │                  │
        └───────────────────┼──────────────────┘
                            ▼
                 Updated Excel Workbook
```

---

## Technologies

### Languages

- Python 3.14

### AI

- OpenAI Responses API
- Prompt Engineering

### Automation

- xlwings
- Microsoft Excel
- Google Workspace

### Development

- Git
- GitHub
- VS Code

---

# Project Structure

```
medicaid-ai-assistant/

├── backups/
├── data/
├── logs/
├── prompts/
│   ├── archive/
│   └── weekly_update_current.txt
│
├── src/
│   ├── main.py
│   ├── excel_manager.py
│   ├── prompt_loader.py
│   └── date_utils.py
│
├── README.md
├── .gitignore
└── .env
```

---

# Version History

## Version 2.1

### Added

- ✅ Migrated from openpyxl to xlwings
- ✅ Preserved Microsoft 365 checkboxes
- ✅ Preserved hyperlinks and formatting
- ✅ AI-generated weekly Medicaid summaries
- ✅ Carry Forward logic
- ✅ Already Updated detection
- ✅ Resident progress tracking
- ✅ Runtime tracking
- ✅ Automatic workbook backups
- ✅ Logging framework
- ✅ Improved terminal interface

---

# Roadmap

## Version 2.2

- 🔄 Complete run logging
- 🔄 Logging helper refactor
- 🔄 Improved save verification
- 🔄 Enhanced error handling
- 🔄 Additional workflow optimization

## Version 2.3

- 🔄 Lawmatics Matter Note integration
- 🔄 Lawmatics Case Update synchronization
- 🔄 Automatic update verification
- 🔄 Excel-to-Lawmatics workflow automation

## Version 3.0

- 🔄 Workflow dashboard
- 🔄 Analytics & reporting
- 🔄 Case metrics
- 🔄 Smart workflow recommendations
- 🔄 Enhanced AI-assisted case management

---

# Impact

This project was built to solve a real operational challenge in long-term care Medicaid case management.

The application transforms shorthand case notes into professional weekly Medicaid summaries while maintaining continuity across weeks, reducing repetitive documentation from **hours of manual work to under one minute**.

Rather than serving as a programming exercise, this project is actively used to improve productivity, documentation consistency, and workflow efficiency in a real-world healthcare environment.

---

# Author

**Linnette Garcia**

Healthcare Operations • Medicaid Compliance • Workflow Automation • AI Integration

Building practical AI tools that solve real business problems.

---

## Disclaimer

This project was developed to improve internal workflow efficiency and documentation consistency. No protected health information (PHI), personally identifiable information (PII), API keys, or proprietary client data are included in this repository.
