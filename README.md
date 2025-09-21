# ✈️ Airline Passenger Compensation Bot

![UiPath](https://img.shields.io/badge/RPA-UiPath-blue?style=for-the-badge\&logo=uipath)
![Automation](https://img.shields.io/badge/Process-Automation-orange?style=for-the-badge)
![Email](https://img.shields.io/badge/Integration-Email-green?style=for-the-badge\&logo=gmail)
![Status](https://img.shields.io/badge/Status-Deployed-success?style=for-the-badge)

---

## 📌 Project Overview

This project is an **individual RPA solution built in UiPath Web Studio** to handle **airline passenger compensation claims** for flight delays and cancellations.

The bot automates the following tasks:

* Extracts passenger details from **PDF attachments** in emails.
* Validates ticket data against **Excel records**.
* Applies compensation rules from a **hidden JSON file**.
* Sends **automated responses** to passengers with calculated compensation amounts.

By using **two agents** and an unattended workflow, the process is streamlined and fully automated.

---

## 🎯 Objectives

* Automate the lifecycle of passenger compensation claims.
* Eliminate manual PDF reading, validation, and email replies.
* Apply consistent and rule-driven compensation calculations.
* Improve passenger satisfaction with quick and transparent processing.

---

## 🛠️ Tools & Technologies

* **UiPath Web Studio** – Automation development
* **PDF Extraction Activities** – To extract text from ticket PDFs
* **JSON File (Hidden)** – For storing compensation rules
* **Excel** – Passenger database for validation
* **Email Integration** – For sending automated responses
* **UiPath Orchestrator (Cloud)** – To deploy as unattended automation
* **GitHub** – For version control and documentation

---

## 📂 Project Structure

```plaintext
Airline-Passenger-Compensation-Bot/
│── Agent1 Airline.uis     # UiPath agent to calculate compensation
│── Airline Agent 2.uis               # UiPath agent to extract PNR & passenger info from PDFs
│── RPA Integration of Airline Project.uid     # RPA workflow to handle email responses
│── CompensationRules.json                  # Hidden JSON rules for compensation policies
│── README.md                               # Project documentation
```

---

## 🚀 Workflow Steps

1. **Email & PDF Processing**

   * Reads incoming passenger emails with attached tickets.
   * Extracts text from the PDF attachment.

2. **PNR Extraction (Agent 2)**

   * Parses the extracted PDF text.
   * Retrieves **PNR** and **passenger details** for validation.

3. **Passenger Validation**

   * Cross-checks extracted details against **Excel records**.

4. **Compensation Calculation (Agent 1)**

   * Loads rules from **CompensationRules.json**.
   * Applies conditions (delays/cancellations) to calculate compensation.

5. **Email Response Workflow**

   * Prepares a response with calculated compensation amount.
   * Sends automated reply to the passenger.

---

## ⚡ How to Run

1. Clone this repository:

   ```bash
   git clone https://github.com/your-username/airline-compensation-bot.git
   ```
2. Open the project in **UiPath Web Studio**.
3. Update configuration files:

   * Provide **Excel passenger database**.
   * Ensure **CompensationRules.json** is in the correct directory.
   * Configure your **email account** in UiPath.
4. Run the workflow in Studio or deploy it as **unattended bot** via Orchestrator.
5. The bot will process passenger claims automatically.

---

## 📊 Example JSON Rule (CompensationRules.json)

```json
{
  "delayed": {
    "2-3_hours": 500,
    "3-5_hours": 1000,
    "5+_hours": 2000
  },
  "canceled": {
    "domestic": 3000,
    "international": 6000
  }
}
```

## ✨ Outcomes & Achievements

* Automated processing of **airline compensation claims**.
* Reduced manual work from hours to minutes.
* Applied **consistent policy rules** via JSON file.
* Increased passenger satisfaction with **fast responses**.
* Showcased **independent UiPath development skills**.

---

## 👤 Author

Developed by **Devupalli Jayanth**

---
