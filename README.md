# Egis Mobile — Electrical Wire Size Calculator (Senior Capstone Project)

A cross-platform mobile application developed for **Egis Mobile** to streamline field operations for mobile equipment technicians. This application replaces manual reference charts with an intelligent, dynamic calculator that computes precise electrical wire sizes based on real-world engineering constraints.

> **Note on Repository Contents:** The source code for this project is proprietary and remains private under a Non-Disclosure Agreement (NDA) with Egis Mobile. This repository serves as a public portfolio detailing the architecture, engineering decisions, and system capabilities.

---

## 🚀 Key Features
* **Dynamic Wire Size Calculator:** Processes user inputs (voltage, current, run length, temperature, and allowable voltage drop) to instantly determine the correct wire gauge.
* **Integrated Documentation Access:** Quick-access portals for the end-user operations guide and administrator maintenance documentation.
* **Admin Database Management Tool:** A secure administrative panel allowing real-time updates to underlying wire spec sheets and database entries.
* **Universal Cross-Platform Deployment:** Engineered utilizing a unified codebase to run seamlessly on both iOS and Android.

## 🛠️ Technical Stack & Architecture
* **Frontend Mobile Framework:** React Native with Expo
* **Language:** TypeScript (Strictly typed for data payload safety)
* **Routing:** File-based navigation via Expo Router
* **State Management:** React Context API for localized calculator input states
* **Database & Cloud:** Firebase Firestore (for storing and syncing QR code spec sheets)

---

## 🧠 Engineering Insights & AI-Powered Workflow

### 1. Navigating Complex Calculation Logic
The core challenge of the app was translating strict electrical formulas and physical wire properties into clean, reactive TypeScript functions. Because calculating voltage drop over varying distances and temperatures requires precise arithmetic, we utilized an **AI-assisted engineering workflow** to accelerate development. 
* **The Process:** We used Google Gemini and GitHub Copilot to rapidly prototype the mathematical utility functions and generate boilerplate UI wrappers for the complex input forms.
* **The Human Code Review:** AI frequently struggled with the strict layout rules of React Native and proper TypeScript interface declarations. I audited the AI-generated outputs, manually resolved state management discrepancies, fixed layout clipping configurations, and implemented rigorous error handling for invalid user inputs.

### 2. UI/UX & Prototyping
To maintain brand alignment and structural consistency, our team prioritized UI/UX design. We built complete high-fidelity mockups in **Figma** using auto-layout, interactive components, and precise grid constraints. This rigorous design phase ensured that moving from a prototype to React Native components yielded pixel-perfect visual fidelity.

### 3. Data Integration & Firestore
We engineered the application to fetch live data from a Firestore database, matching incoming queries against a schema mapping out `Egis Mobile Electric QR Spec Sheets`. This allows administrators to push real-time updates to the mobile application without requiring a new App Store build.
<img width="696" height="740" alt="egis" src="https://github.com/user-attachments/assets/687d2bcb-e32d-42a3-a402-10433f28cdbb" />


---

## 👥 Professional Team Collaboration
This application was engineered over a multi-month lifecycle as part of a Senior Engineering Capstone project. I collaborated directly with my development team, academic faculty advisors, and the Project Director at Egis Mobile to ensure all enterprise requirements, software testing criteria, and project deadlines were met perfectly.
