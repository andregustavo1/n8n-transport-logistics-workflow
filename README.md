# n8n Driver Commission Automation

This repository contains an **n8n automation workflow** designed for a logistics/transportation company to automate the **weekly commission calculation for fleet drivers**.

## 🧠 Problem Solved

Previously, the finance team manually processed all weekly loads and calculated each driver's commission in a spreadsheet. This was time-consuming and error-prone.

With this automation:
- Driver data is fetched automatically from the webhook.
- Loads completed during the week are processed.
- Data is inserted into a Google Sheet.
- Commission and totals are calculated automatically.

## ⚙️ Workflow Overview

- **Trigger**: Webhook receives weekly data.
- **Conditions**: Verifies if the data is from a group and if the message contains a fleet driver.
- **Processing**: 
  - AI Agent Extracts JSON
  - Gets the week number
  - Uses multiple Switch nodes to send data to the correct Google Sheet week
- **Output**: Each driver's weekly commissions are updated in the corresponding spreadsheet.

## 📸 Workflow Preview
![image](https://github.com/user-attachments/assets/b6cb250b-eb54-4109-b895-590f3b80fad3)
