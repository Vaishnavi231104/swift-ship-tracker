# SwiftShip Tracker CRM — Enterprise Logistics AI Solution

## 📌 Project Overview
SwiftShip Tracker is a scalable, end-to-end CRM solution built within a Salesforce Developer Org designed to manage the comprehensive parcel lifecycle—spanning from booking and dispatch to real-time conversational AI tracking and final delivery confirmation[cite: 5, 6]. 

The architecture bridges critical visibility gaps by automating milestone updates, securing multi-tenant customer data, and introducing conversational intelligence via Salesforce Agentforce[cite: 6].

## 📂 Core Project Deliverables
All project requirements, architectural configurations, schema screenshots, and code components are fully consolidated into a single, comprehensive PDF document[cite: 5].

- **📥 Complete Documentation:** [Click here to view or download SWIFT_SHIP_TRACKER_DOCUMENTATION.pdf](SWIFT_SHIP_TRACKER_DOCUMENTATION.pdf)[cite: 5]
- **🎥 Presentation Demo Video:** [Insert Link to your Google Drive, Loom, or YouTube presentation here][cite: 5]

---

## 🏗️ Technical Architecture Highlights
- **Relational Schema:** Custom entities including `Parcel__c`, `Delivery__c`, `Sender__c`, and `Receiver__c` engineered for seamless transaction tracing[cite: 5, 6].
- **Automations:** Event-driven Record-Triggered Flows, supervisor Approval Processes, Scheduled Actions, and Apex database triggers[cite: 5, 6].
- **Security Matrix:** Baseline Organization-Wide Defaults (OWD) locked strictly to Private, configured with an explicit corporate Role Hierarchy tree[cite: 5, 6].
- **AI Core Integration:** Agentforce AI Field Generation Prompts mapped via the Einstein Prompt Builder framework[cite: 5, 6].

---

## 🧪 Functional Testing Matrix
The project passes all automated test cases with 100% code coverage metrics[cite: 6]. Manual validation runs verify all underlying system hooks:

| Feature Evaluated | Mock System Inputs Passed | Expected Functional Outcome |
| :--- | :--- | :--- |
| **Validation Rule** | `Weight__c = -10` | Database insert is blocked; page throws validation message[cite: 4, 5]. |
| **Apex Core Trigger** | `Weight__c = 30` | Automatically stamps description with heavyweight priority message[cite: 4, 5]. |
| **Approval Wizard** | `Weight__c = 55` | Record auto-locks and routes straight to supervisor pending review queue[cite: 4, 5]. |
| **Agentforce AI** | `ids = P-001` | Parses intent flawlessly and returns dynamic language tracking cards[cite: 4, 5]. |

---

## 🚀 Future Enhancements Roadmap
- **Portal Chatbot Widget:** Deploying the active tracking prompt template straight onto web communities for immediate automated self-service[cite: 5, 6].
- **Lightning Web Components (LWC):** Assembling graphical route maps to visually plot logistics coordinates directly on screen[cite: 5, 6].mbling graphical route maps to visually map logistics directly on screen[cite: 7].e
