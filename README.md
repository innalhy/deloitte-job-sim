## Deloitte Job Simulation - Daikibo Machine Telemetry Dashboard 📊

### Project Overview
This repository contains the completed deliverables for **Task 1** and **Task 2** of the Deloitte Technology Job Simulation, focused on building a private machine health telemetry dashboard for Daikibo manufacturing facilities.

Daikibo operates 4 factories, each with 9 monitored industrial machines. The solution standardises two different telemetry JSON formats into a unified structure, plus a formal project proposal and implementation planning for a secure internal machine health dashboard.

### Task 1: Telemetry Data Format Conversion 🧩
#### What I Completed: 
- Created Python `main.py` to convert two different telemetry JSON input formats into one unified standard output format.
- Built two core conversion functions:
  - `convertFromFormat1()` — Parses concatenated string location, maps flat telemetry fields into unified schema.
  - `convertFromFormat2()` — Parses nested device/location/data structure, converts ISO timestamp to epoch milliseconds.
- Implemented unit testing with `unittest` to validate conversion against the expected `data-result.json`.
- Handled schema mapping, string splitting, timestamp conversion, and nested object reconstruction.
- All unit tests pass after fixing schema structure, key mapping and nested data object formatting issues.

#### Files Included:
- `main.py` — Core conversion logic + unit tests
- `data-1.json` — Telemetry input Format 1
- `data-2.json` — Telemetry input Format 2
- `data-result.json` — Unified target output format

### Task 2: Formal Development Proposal & Project Timeline 📝

#### What I Completed:
Authored a formal, structured development proposal for the Daikibo private machine health dashboard, including all required sections:
- Overview — High-level project introduction and purpose
- Scope — Defined dashboard functionality, intranet-only access, internal SSO authentication, single-page UI, collapsible factory/device views with status history
- Man-hour Estimate — Breakdown for development, testing and system integration
- Project Timeline & Milestones — 4-week / 20 business day structured plan
- Ongoing Support — Post-launch bug fixes, support tickets, and future feature enhancements

#### Dashboard Core Features (Defined in Proposal)
- Private access restricted **only to Daikibo internal intranet** 🔒
- Authentication synced to company internal auth server (use existing corporate accounts)
- Single-page dashboard showing real-time health status of all 36 machines
- Collapsible / expandable view at factory level and individual device level
- Historical machine status timeline view for each device

### How to Run Task 1 ▶️
1. Clone the repo
2. Ensure `data-1.json`, `data-2.json`, `data-result.json` are in the same folder as `main.py`
3. Run:
```bash
python main.py
```
4. All unit tests will execute and confirm successful format conversion.

### Skills Demonstrated ✅
- Python JSON data parsing & transformation
- Unit testing and debugging
- Data schema standardisation
- Formal technical proposal writing
- Project scoping, work estimation and milestone timeline planning
- Requirements analysis and solution design for enterprise internal dashboards