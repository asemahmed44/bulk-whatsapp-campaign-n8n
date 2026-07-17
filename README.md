# 🚀 Automated Bulk WhatsApp Campaign Engine

An advanced enterprise-ready automation workflow built with **n8n** and **Evolution API**[cite: 1]. This engine allows users to trigger mass WhatsApp marketing campaigns via an interactive web form, featuring dynamic data parsing, automated contact sanitization, and intelligent anti-ban message randomization.

---

## 🔥 Key Features

* **Interactive Campaign Form:** Seamless multi-field n8n form trigger for uploading spreadsheets and configuring templates on the fly[cite: 1].
* **Anti-Ban Message Randomization:** Supports multiple template alternatives (up to 3 variations) and dynamically randomizes message selection to heavily reduce WhatsApp banning risks[cite: 1].
* **Dynamic Content Personalization:** Automatically parses text fields to substitute template strings like `{{name}}` with customized contact data[cite: 1].
* **Automated Data Normalization:** Smart JavaScript processing to strip non-numeric characters from phone numbers and handle flexible column mapping (`name`, `Name`, `phone`, `mobile`, etc.)[cite: 1].
* **Built-in Rate Limiting:** Implements a controlled 3-second batching delay to comply with messaging safety best practices[cite: 1].

---

## 🛠️ Architecture & Tech Stack

* **Core Engine:** n8n Workflow Automation[cite: 1].
* **Gateway API:** Evolution API (WhatsApp Integration)[cite: 1].
* **Logic Layer:** JavaScript (Custom parsing, data normalization, and randomization logic)[cite: 1].

---

## 📋 Prerequisites

Before deploying this workflow, ensure you have access to:
1. An active **n8n** instance.
2. An active **Evolution API** instance with an authenticated WhatsApp instance gateway.

---

## 💻 Installation & Deployment

1. **Download the Source:** Clone this repository or download the `bulk-whatsapp-campaign-n8n.json` file.
2. **Import into n8n:** Open your n8n dashboard, create a new workflow, click on **Import from File**, and select the JSON file (or simply copy-paste the raw JSON directly into the canvas)[cite: 1].
3. **Configure Gateway Credentials:** Open the `Evolution API - Send Text` node and link your validated `evolutionApi` credentials[cite: 1].
4. **Set Instance Configuration:** Update the `instanceName` parameter (Default is set to `HDL`) within the node parameters according to your designated target session[cite: 1].
5. **Activate & Launch:** Switch the workflow status to **Active**, grab the generated Form URL, and launch your automated campaign.
