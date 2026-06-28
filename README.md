# SwiftShip Tracker — Salesforce AI Service Agent CRM

An autonomous, AI-driven package tracking solution built on the Salesforce platform using **Agentforce Service Agents**, **Prompt Builder**, and **Autolaunched Flows**. This project was developed as part of the **Salesforce Developer Track** virtual internship powered by **SkillWallet**.

---

## 🚀 Project Overview
The **SwiftShip Tracker** addresses high-volume customer support inquiries by automating the entire parcel status tracking lifecycle. Instead of waiting for human support agents, customers interact with an intelligent, conversational AI Service Agent. The agent dynamically queries a custom relational database schema, retrieves target shipment logistics, and delivers real-time, line-by-line formatted updates instantly.

### Key Business Values
* **Zero-Touch Resolution:** Automatically resolves routine shipment inquiries without human agent intervention.
* **Streamlined Analytics:** Provides immediate operational insights into package distribution statuses and shipping trends.
* **Enhanced Security:** Restricts autonomous AI database access to explicit object-level read-only parameters.

---

## 🏗️ Core Architecture & Features

### 1. Data Model & Schema (Backend)
Built completely within a Salesforce Developer Edition environment, the database features robust relational custom object tracking:
* **`Parcel__c`**: The primary custom object tracking critical logistics.
  * `Parcel_Name__c` (Text/Auto-Number) — Internal identifier name.
  * `Parcel_ID__c` (Text) — Unique customer-facing tracking number (e.g., `P-001`).
  * `Status__c` (Picklist) — Tracks lifecycle stage (`Ordered`, `In Transit`, `Out for Delivery`, `Delivered`).
  * `Weight__c` (Number) — Cargo weight details.
  * `Estimated_Delivery__c` (Date) — Scheduled arrival timeline.
* **`Delivery__c`**: Relational custom object tracking distribution logs and regional milestone records.

### 2. Business Process Automation (Flows)
* **Autolaunched Data Engine:** A background Salesforce Flow acts as the security and retrieval layer. It takes the text tracking string provided by the customer, queries the `Parcel__c` database, filters records to find an exact match, and securely maps the output record data back to the prompt framework.

### 3. Generative AI & Prompt Engineering
* **Prompt Templates:** Engineered in Salesforce **Prompt Builder** to ground the Large Language Model (LLM) with real-time record variables while enforcing a strict text-formatting blueprint.
* **Agentforce Actions:** The Prompt Template is encapsulated into a custom **Agent Action (Tool)**, explicitly instructed with natural language capabilities so the Agent knows exactly when to execute the tracking engine during customer conversations.

### 4. Robust Security Framework
* **`SwiftShip` Permission Set:** Deployed to grant explicit `Read` and `View All Records` object permissions to the background integration user profile (**Einstein Agent User**), bypassing standard system access denials and ensuring reliable execution.

---

## 📁 Project Deliverables

This repository contains the full suite of deployment files and documentation required for final evaluation:

* 📄 **`SwiftShip_Tracker_Documentation.pdf`**: A professional, comprehensive technical design document covering Requirement Analysis (Phase 1) through Deployment & Testing (Phases 4 & 5). Includes deep architectural details and configuration UI screenshots.
* 🎥 **Demo Video Presentation**: A detailed video walkthrough explaining the backend schema, background flow architecture, permission settings, and a live end-to-end user interface chat execution.
  * 🔗 **[Watch the Project Demo Video Here](PASTE_YOUR_GOOGLE_DRIVE_OR_YOUTUBE_LINK_HERE)**

---

## 📦 Unmanaged Package Installation

The core database model, automation parameters, and permission frameworks have been securely bundled into a native Salesforce Unmanaged Package. System administrators can deploy this foundational architecture directly into an alternate Salesforce Environment or Sandbox:

➡️ **[Click Here to Install the SwiftShip Tracker Package]((https://login.salesforce.com/packaging/installPackage.apexp?p0=04tgL000000Hv1t))**

*Note: If you encounter a namespace collision warning during testing, please ensure you are installing the package into a separate Salesforce testing environment or playground, as Salesforce blocks installing unmanaged packages back into their native source org.*

---

## 🛠️ Environment & Tools
* **Platform:** Salesforce Developer Edition (Summer '26 Release)
* **AI Framework:** Salesforce Agentforce & Einstein Prompt Builder
* **Automation:** Salesforce Flow Builder
* **Analytics:** Salesforce Reports & Dashboards Engine
