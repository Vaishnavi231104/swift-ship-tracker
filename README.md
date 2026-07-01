# SwiftShip Tracker CRM — Enterprise Logistics AI Solution

## 📌 Project Overview
SwiftShip Tracker is a scalable, end-to-end CRM solution built within a Salesforce Developer Org designed to manage the comprehensive parcel lifecycle—spanning from booking and dispatch to real-time conversational AI tracking and final delivery confirmation. 

The architecture bridges critical visibility gaps by automating milestone updates, securing multi-tenant customer data, and introducing conversational intelligence via Salesforce Agentforce[cite: 7].

### 🎯 Primary Objectives
- **Operational Automation:** Eliminate manual package status tracking overhead via event-driven Flows and Apex handlers[cite: 7].
- **Agentforce AI Integration:** Provide transparent, conversational tracking utilities to users via generative prompt modeling[cite: 7].
- **Zero-Trust Security:** Enforce tight vertical reporting and data privacy constraints via role hierarchies and Private Organization-Wide Defaults (OWD)[cite: 7].

---

## 🛠️ Tech Stack & Features Planned
- **Platform Base:** Salesforce Developer Org[cite: 7]
- **Declarative Tools:** Record-Triggered Flows, Scheduled Flows, Auto-Launched Subflows, and Approval Processes[cite: 7]
- **Programmatic Layer:** Apex Triggers, Apex Handler Classes, and Async Apex[cite: 7]
- **AI Framework:** Agentforce AI Engine & Einstein Prompt Builder[cite: 7]
- **UI Framework:** Lightning App Console & Responsive Dynamic Forms[cite: 7]
- **Data Security:** Profiles, Permission Sets, OWD Private, and Sharing Rules[cite: 7]

---

## 🏗️ Architectural Framework

### Data Model Design (Schema Builder Overview)
The platform relational schema maps clear pathways across standard and custom entities[cite: 7]:
- `Parcel__c` (Custom Object): Core ledger tracking weight, status picklists, and dimensions[cite: 7].
- `Delivery__c` (Custom Object): Operational runtime tracking route coordinates and warehouse hubs[cite: 7].
- `Sender__c` & `Receiver__c` (Custom Objects): Isolates origin and destination profile communication metrics[cite: 7].

### Access Controls & Role Hierarchy
- Global OWD permissions are locked down completely to **Private**[cite: 7].
- Upward vertical data visibility scales explicitly based on organizational tiers:
  `Amity University Root ➔ Delivery Manager ➔ Delivery Agent ➔ Customer`[cite: 7].

---

## 🧪 Functional Testing Matrix
The project passes all automated test cases with **100% code coverage** metrics[cite: 7]. Manual validation runs verify all underlying system hooks:

| Feature Evaluated | Mock System Inputs Passed | Expected Functional Outcome |
| :--- | :--- | :--- |
| **Validation Rule** | `Weight__c = -10` | Database insert is blocked; page throws validation message[cite: 7]. |
| **Apex Core Trigger** | `Weight__c = 30` | Automatically stamps description with heavyweight priority message[cite: 7]. |
| **Approval Wizard** | `Weight__c = 55` | Record auto-locks and routes straight to supervisor pending review queue[cite: 7]. |
| **Agentforce AI** | `ids = P-001` | Parses intent flawlessly and returns dynamic language tracking cards[cite: 7]. |

---

## 🎥 Project Presentation Walkthrough
- **Demo Video Presentation:** [Insert Link to your Drive, Loom, or YouTube Unlisted video here][cite: 6]
- **Comprehensive Report Deliverable:** Found under `documentation/SWIFT_SHIP_TRACKER_DOCUMENTATION.pdf`

---

## 🚀 Future Enhancements Roadmap
- **Portal Chatbot Widget:** Deploying the active tracking prompt template straight onto web communities[cite: 7].
- **Lightning Web Components (LWC):** Assembling graphical route maps to visually map logistics directly on screen[cite: 7].e
