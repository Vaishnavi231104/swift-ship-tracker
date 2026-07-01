# SwiftShip Tracker CRM — Enterprise Logistics AI Solution

## 📌 Project Overview
SwiftShip Tracker is a scalable, end-to-end CRM solution built within a Salesforce Developer Org designed to manage the comprehensive parcel lifecycle—spanning from booking and dispatch to real-time conversational AI tracking and final delivery confirmation. 

The architecture bridges critical visibility gaps by automating milestone updates, securing multi-tenant customer data, and introducing conversational intelligence via Salesforce Agentforce.

## 📂 Core Project Deliverables
All project requirements, architectural configurations, schema screenshots, and code components are fully consolidated into a single, comprehensive PDF document.

- **📥 Complete Documentation:** [Click here to view or download SWIFT_SHIP_TRACKER_DOCUMENTATION.pdf](SWIFT_SHIP_TRACKER_DOCUMENTATION.pdf)
- **🎥 Presentation Demo Video:** [Insert Link to your Google Drive, Loom, or YouTube presentation here]

---

## 🏗️ Technical Architecture Highlights
- **Relational Schema:** Custom entities including `Parcel__c`, `Delivery__c`, `Sender__c`, and `Receiver__c` engineered for seamless transaction tracing.
- **Automations:** Event-driven Record-Triggered Flows, supervisor Approval Processes, Scheduled Actions, and Apex database triggers.
- **Security Matrix:** Baseline Organization-Wide Defaults (OWD) locked strictly to Private, configured with an explicit corporate Role Hierarchy tree.
- **AI Core Integration:** Agentforce AI Field Generation Prompts mapped via the Einstein Prompt Builder framework.

---

## 🧪 Functional Testing Matrix
The project passes all automated test cases with 100% code coverage metrics. Manual validation runs verify all underlying system hooks:

| Feature Evaluated | Mock System Inputs Passed | Expected Functional Outcome |
| :--- | :--- | :--- |
| **Validation Rule** | `Weight__c = -10` | Database insert is blocked; page throws validation message. |
| **Apex Core Trigger** | `Weight__c = 30` | Automatically stamps description with heavyweight priority message |
| **Approval Wizard** | `Weight__c = 55` | Record auto-locks and routes straight to supervisor pending review queue |
| **Agentforce AI** | `ids = P-001` | Parses intent flawlessly and returns dynamic language tracking cards |

---

## 🚀 Future Enhancements Roadmap
- **Portal Chatbot Widget:** Deploying the active tracking prompt template straight onto web communities for immediate automated self-service.
- **Lightning Web Components (LWC):** Assembling graphical route maps to visually plot logistics coordinates directly on screen.
