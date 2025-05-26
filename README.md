**🩺 DCR Insights Dashboard – Power BI + SSAS Tabular Live Connection**

This repository contains the Doctor Call Report (DCR) Dashboard, developed in Power BI with a live connection to SSAS, to analyze call activity, target performance, and doctor coverage by division, zone, and brand.


**🧩 Data Model Overview**
The model follows a clean star schema structure, connecting key tables:

1. Call entry records (PBI_DCR_COMBINED_SRC_T)
2. Doctor master list
3. Market and team hierarchies
4. Product and category dimensions
5. A custom calendar table for time-based slicing


**⚙️ Dashboard Features**
🧠 Live connected model from SSAS for real-time analytics

📅 Interactive date range filtering (by day, month, etc.)

📍 Visual breakdowns by Market Team, Division, Zone, Region, Brand, Business Type


**📈 Key Metrics:**
1. Total Active MIOs vs. Submitted DCRs
2. Target Doctor and Doctor Visit performance
3. Doctor Coverage %
4. Division/Zone/Region/Brand-level performance
5. MIO Call Efficiency metrics


**🗂 Suggested Folder Structure**

powerbi-dcr-dashboard/
├── README.md
├── Model/
│   └── Model.bim                      # SSAS model (Tabular Editor export)
├── Documentation/
│   ├── DCR Dashboard.png              # Screenshot of dashboard
│   ├── Model Diagram.PNG              # Data model image
│   └── UserGuide.md                   # End-user instructions
├── SSASConnection/
│   └── connection_config.json         # SSAS connection info (sanitized)
├── Scripts/
│   └── refresh_api_trigger.ps1        # Optional auto-refresh script


**🔧 Tools and Technologies**
1. Power BI Desktop
2. SQL Server Analysis Services (Tabular)
3. DAX
4. GitHub for version control
5. Tabular Editor (for model export)


**📦 How to Use**
Clone the repo:
1. git clone https://github.com/YOUR_USERNAME/powerbi-dcr-dashboard.git
2. Open Power BI and connect to the SSAS model as described in SSASConnection/connection_config.json
3. Load and analyze using filters for date, brand, region, zone, and doctor types
4. Publish to Power BI Service for distribution


**🚫 Notes**
1. .pbix file not included due to large size and SSAS live dependency
2. No credentials or sensitive information are stored in the repo
3. Ensure secure SSAS access for full functionality

 
