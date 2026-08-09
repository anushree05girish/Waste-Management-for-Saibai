# Dugong Dispose: Digital Education for Waste Management on Saibai Island 🌊🚮

> **Engineers Without Borders (EWB) Challenge 2024 Project Report**  
> **Course:** Introduction to Engineering Projects  
> **Group Name:** EDTECH DUGONGS (Tutorial 01, Zone Blue)  
> **Design Area:** 6. ICT | **Opportunity 6.3:** Language, knowledge preservation, and digital education tools  
> **GitHub Profile:** [anushree05girish](https://github.com/anushree05girish)

---

## 📌 Executive Summary & Project Overview

**Dugong Dispose** is an interactive, multi-lingual digital mobile application designed to educate, engage, and empower the Indigenous community on Saibai Island (Torres Strait) towards sustainable waste management practices. 

Saibai Island faces severe waste management challenges due to its remote geographic location, low-lying topography, limited infrastructure, and vulnerable marine ecosystem. The **Dugong Dispose** platform bridges critical knowledge gaps by presenting waste disposal guidance in English, local Saibai languages, and Torres Strait Creole, tailored across all age demographics.

```mermaid
graph TD
    %% Custom Styling
    classDef primary fill:#0077b6,stroke:#03045e,stroke-width:2px,color:#fff;
    classDef highlight fill:#00b4d8,stroke:#0077b6,stroke-width:2px,color:#fff;
    classDef accent fill:#90e0ef,stroke:#0077b6,stroke-width:1px,color:#03045e;
    classDef success fill:#52b788,stroke:#2d6a4f,stroke-width:2px,color:#fff;

    SubGraph1["<b>🌏 Saibai Island Environment</b>"]
    A["<b>Geographic Isolation & Coastal Vulnerability</b>"] ::: primary
    B["<b>Limited Infrastructure & Biosecurity Constraints</b>"] ::: primary
    end

    SubGraph2["<b>📱 Dugong Dispose Digital Solution</b>"]
    C["<b>Multi-Lingual Educational Platform</b><br/>(Kalaw Kawaw Ya | Yumplatok | English)"] ::: highlight
    D["<b>Interactive App Modules</b><br/>(Monitoring, Rewards, Waste Map, Forum)"] ::: highlight
    end

    SubGraph3["<b>🌱 Desired Impact & Outcomes</b>"]
    E["<b>Increased Waste Segregation & Recycling</b>"] ::: success
    F["<b>Protection of Marine Life & Dugong Habitats</b>"] ::: success
    G["<b>Empowered Community & Eco-Habits</b>"] ::: success
    end

    A --> C
    B --> C
    C --> D
    D --> E
    D --> F
    D --> G
```

---

## 🎯 How Might We (HMW) Statement

> *"How might we effectively educate and engage the Saibai community on sustainable waste management practices in order to increase awareness and adoption of effective waste management methods?"*

---

## 🏗️ System Architecture & Data Flow

```mermaid
flowchart TB
    %% Nodes definition
    user[("👤 Community Residents & Youth")]
    app["📱 Dugong Dispose Mobile App<br/>(iOS / Android / Offline Cache)"]
    backend["☁️ Cloud & Analytics Backend<br/>(Telstra 4G Cellular Network)"]
    council["🏛️ TSIRC & Local Council Dashboard"]
    logistics["🚢 Waste Logistics & Porter Service<br/>(Sea Swift / CEQ Recycling)"]

    %% Flow interactions
    user -->|"1. Segregates waste & scans QR / drops off"| app
    user -->|"2. Reports waste hotspots via photo map"| app
    app -->|"3. Earns reward points & views tutorials"| user
    app <-->|"4. Syncs data & alerts over Telstra 4G"| backend
    backend -->|"5. Hotspot & bin fill-level analytics"| council
    council -->|"6. Optimized waste collection schedules"| logistics

    %% Styling
    style user fill:#023e8a,stroke:#03045e,color:#fff
    style app fill:#0077b6,stroke:#03045e,color:#fff
    style backend fill:#0096c7,stroke:#03045e,color:#fff
    style council fill:#00b4d8,stroke:#03045e,color:#fff
    style logistics fill:#48cae4,stroke:#03045e,color:#111
```

---

## ✨ Key Features & Application Modules

```mermaid
mindmap
  root((Dugong Dispose Platform))
    📊 Waste Monitoring System
      Household trend tracking
      Public area bin status
      Optimized collection schedules
    🎁 Rewards Incentive System
      Points for waste segregation
      Discount on waste disposal fees
      Community recognition & rewards
    💬 In-App Community Forum
      Eco-friendly tips & updates
      Community clean-up events
      Resident discussion board
    🔔 Smart Notification Alerts
      Bin collection timing alerts
      Clean-up drive reminders
      Multi-lingual educational highlights
    🎮 Gamified Map & Mini-Games
      Interactive hotspot waste map
      Youth-focused sorting games
      Culturally tailored marine protection lessons
```

1. **📊 Waste Monitoring System**
   - Tracks waste generation trends across households and public areas.
   - Provides real-time insights to local council and community members for optimized collection schedules.

2. **🎁 Rewards-Based Incentive System**
   - Encourages community participation by awarding points for proper waste segregation and recycling.
   - Points can be redeemed for local community rewards or discount incentives on waste disposal fees ($10 to $8 reduction).

3. **💬 In-App Community Forum**
   - Enables residents to post waste-related updates, share eco-friendly tips, arrange community clean-ups, and voice environmental concerns.

4. **🔔 Smart Notification Alerts**
   - Sends timely updates regarding bin pick-up times, community clean-up drives, and educational highlights.

5. **🎮 Gamified Waste Map & Educational Mini-Games**
   - Interactive map featuring gamified challenges specifically tailored to engage youth (Gen-Z / children).
   - Teaches waste sorting and marine protection through fun, culturally relevant mechanics.

---

## ⚖️ Design Decision Matrix Analysis

```mermaid
gantt
    title Design Option Evaluation Scores (Out of 5)
    dateFormat  X
    axisFormat %s

    section Design Option 1: Smart Bins & Sensors
    Implementation Cost (Low=5)     : active, 1, 0, 1
    Maintenance Demand (Low=5)      : active, 2, 0, 2
    Daily Functionality              : active, 4, 0, 4
    Accessibility                    : active, 3, 0, 3
    Simplicity                       : active, 2, 0, 2
    Environmental Impact             : active, 4, 0, 4
    Community Engagement             : active, 3, 0, 3
    Cultural Relevance               : active, 3, 0, 3

    section Design Option 2: Digital Storytelling & Podcasts
    Implementation Cost (Low=5)     : crit, 4, 0, 4
    Maintenance Demand (Low=5)      : crit, 4, 0, 4
    Daily Functionality              : crit, 3, 0, 3
    Accessibility                    : crit, 3, 0, 3
    Simplicity                       : crit, 4, 0, 4
    Environmental Impact             : crit, 3, 0, 3
    Community Engagement             : crit, 4, 0, 4
    Cultural Relevance (Ethics Risk) : crit, 1, 0, 1

    section Design Option 3: Dugong Dispose Mobile App (Selected)
    Implementation Cost (Low=5)     : done, 3, 0, 3
    Maintenance Demand (Low=5)      : done, 4, 0, 4
    Daily Functionality              : done, 5, 0, 5
    Accessibility                    : done, 5, 0, 5
    Simplicity                       : done, 4, 0, 4
    Environmental Impact             : done, 4, 0, 4
    Community Engagement             : done, 5, 0, 5
    Cultural Relevance               : done, 5, 0, 5
```

### 🗑️ Physical Color-Coded Waste Bin Infrastructure Integration

To complement the mobile app, a physical 4-category color-coded bin system (adapted for local conditions) is established at community hotspots:

```
┌─────────────────────────┬─────────────────────────┬─────────────────────────┬─────────────────────────┐
│     🟢 GREEN BIN        │     🟡 YELLOW BIN       │       🔴 RED BIN        │       🔵 BLUE BIN       │
├─────────────────────────┼─────────────────────────┼─────────────────────────┼─────────────────────────┤
│ Organic Garden Waste &  │ Recyclable Metals,      │ Burnable / Combustible  │ Non-Burnable Materials  │
│ Vegetation              │ Plastics & Glass        │ Non-Recyclable Waste    │ Safe for Incineration   │
└─────────────────────────┴─────────────────────────┴─────────────────────────┴─────────────────────────┘
```

---

## 💰 Project Budget & Cost Breakdown

The overall estimated budget for **Dugong Dispose** is **$288,810.14 AUD** for complete development and rollout, with an ongoing maintenance budget of **$6,994.41 AUD/year**.

```mermaid
pie title Budget Allocation Breakdown ($288,810.14 AUD)
    "App Software Development & Design" : 240000.00
    "Hardware & Bin Infrastructure" : 28500.00
    "Posters & Community Brochures" : 4200.00
    "Freight & Logistics to Saibai Island" : 11110.14
    "Community Workshops & Outreach" : 5000.00
```

| Expense Category | Description & Scope | Cost (AUD) |
| :--- | :--- | :--- |
| **Software Development** | 6-Month Agile development (PM, UI/UX, iOS/Android Devs, QA) | $240,000.00 |
| **Physical Infrastructure** | Color-coded 4-bin sets for 15 primary community hotspots | $28,500.00 |
| **Educational Materials** | 73 Household brochures + 15 Community hotspot QR posters | $4,200.00 |
| **Logistics & Freight** | Marine barge transport (Sea Swift) to remote Saibai Island | $11,110.14 |
| **Outreach & Translation** | Community elder collaboration & TSIRC workshops | $5,000.00 |
| **Total Initial Investment**| **Full Initial Project Deployment** | **$288,810.14** |
| **Annual Maintenance** | Ongoing bug fixes, Telstra 4G cloud hosting & updates | **$6,994.41 / year** |

---

## 👥 Team Members & Contributions

| Student Name | Student ID | Mid-Semester Contributions | End-Semester Contributions |
| :--- | :--- | :--- | :--- |
| **Anushree Girish** | **25415098** | Design Solution Options | Executive Summary + Prototyping |
| **YuetTing Wong** | 25498852 | Project Scope | Detailed Design |
| **Riley Backhouse** | 25358829 | Introduction | Implementation Plan |
| **Michelle Pham** | 24521318 | Proposed Design Solution | Cost Analysis |
| **Sungjin Cho** | 25582065 | Conclusion | Discussion |
| **Mahaba Kamal** | 25579196 | Background | Prototyping |

---

## 🛠️ Implementation & Rollout Timeline

```mermaid
gantt
    title Dugong Dispose 6-Month Project Implementation Schedule
    dateFormat  YYYY-MM-DD
    section Phase 1: Planning
    Stakeholder Engagement & EWB Review   :2024-01-01, 30d
    Cultural Translation & Content Prep   :2024-01-15, 30d
    section Phase 2: App Development
    UI/UX Design & Wireframing           :2024-02-01, 30d
    Frontend & Backend Development        :2024-03-01, 60d
    Testing & QA Validation              :2024-04-15, 30d
    section Phase 3: Infrastructure
    Bin & Poster Procurement              :2024-04-01, 30d
    Sea Swift Transport to Saibai        :2024-05-01, 20d
    Hotspot Installation                 :2024-05-20, 15d
    section Phase 4: Launch & Operations
    Community Workshops & App Rollout     :2024-06-01, 30d
    Post-Launch Maintenance & Support    :2024-07-01, 60d
```

- **Material Sourcing & Marketing:** Posters integrated with QR codes distributed across 15 high-traffic locations on Saibai Island for seamless app access and sign-ups. Color-coded bin systems introduced alongside educational media.
- **Stakeholder Collaboration:** Developed in direct alignment with EWB, Torres Strait Island Regional Council (TSIRC), local elders, and residents.
- **Sustainability & Maintenance:** Long-term app maintenance handled through council partnerships with periodic content updates based on user feedback.

---

## 📁 Repository Structure

```text
.
├── README.md                                       # Comprehensive Project Documentation with Mermaid Diagrams & Data Visuals
└── Assessment Task 2b_ EWB Challenge Team Report.pdf  # Full Project Engineering Report (PDF)
```

---

## 📄 License & Acknowledgements

We acknowledge the Traditional Custodians of the land on Saibai Island, the **Koeybuway** and **Moegibuway** peoples, and pay our respects to their Elders past, present, and emerging. Developed as part of the EWB Challenge 2024 for Introduction to Engineering Projects.
