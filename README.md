# 🎥 Automated YouTube Metadata Extraction Workflow with n8n ⚙️

This project implements an **automated workflow** to extract, enrich, and validate metadata from YouTube videos using **n8n**. The workflow integrates **Microsoft Azure OAuth2** authentication with the **YouTube Data API v3** and **Microsoft Excel 365** via Graph API to collect reliable ground-truth metadata from YouTube at scale. This supports research on enhancing automatic metadata generation through multimodal contextual analysis.

---

## ✨ Features

- ⚡ **End-to-End Automation:** Automatically collect YouTube video metadata (title, description, hashtags) from URLs stored in Excel.  
- 📊 **Microsoft Excel Integration:** OAuth2-secured connection to Excel 365 for dynamic dataset management.  
- 📡 **YouTube Data API v3:** Fetch detailed video metadata for benchmarking and validation.  
- 🧩 **n8n Workflow Orchestration:** Custom JavaScript regex extracts video IDs, automates API calls, parses responses, and enriches datasets.  
- 🗂️ **Dataset Enrichment:** Outputs updated Excel files ready for research use.

---

## 🗂️ Project Structure

- `n8n-workflow.json` - Exported n8n workflow file.  
- `docs/` - Documentation and setup guides.  
- `examples/` - Sample Excel datasets (input and output).  
- `scripts/` - Custom JS functions and regex.

---

## 🚀 Getting Started

### 📋 Prerequisites

- n8n installed locally or use n8n Cloud  
- Google Cloud Console with YouTube Data API v3 enabled and credentials  
- Microsoft Azure subscription with OAuth2 app registered for Microsoft Graph API  
- Microsoft Excel 365 workbook containing YouTube video URLs

### 🔧 Setup Overview

1. 📥 **Install n8n:** See [n8n docs](https://docs.n8n.io/getting-started/installation)  
2. 🔑 **Google API:** Enable YouTube Data API and create credentials  
3. 🛡️ **Azure Setup:** Register app, configure OAuth2, and assign MS Graph permissions  
4. 🔄 **Import Workflow:** Load `n8n-workflow.json` into your n8n instance  
5. 🔐 **Configure Credentials:** Set OAuth2 credentials in n8n for YouTube & Excel  
6. 📥 **Upload Excel:** Add your video URL dataset  
7. ▶️ **Run Workflow:** Trigger manually or schedule automations

---

## 📝 Usage

- Reads YouTube URLs from Excel, extracts video IDs 🎯 via regex  
- Calls YouTube Data API v3 to retrieve metadata 🎞️  
- Parses and structures metadata JSON  
- Writes enriched data back to Excel ✅  
- Includes error handling and logging 🔍

---

## 🛠 Technologies Used

- [n8n](https://n8n.io/) — Workflow automation  
- [YouTube Data API v3](https://developers.google.com/youtube/v3) — Video metadata  
- [Microsoft Graph API](https://developer.microsoft.com/en-us/graph) — Excel integration  
- Microsoft Azure OAuth2 — Secure API access  
- JavaScript — Custom functions & regex  
- Microsoft Excel 365 — Dataset management

---

## 🤝 Contribution

Contributions are welcome! Feel free to open issues or submit pull requests to improve the workflow or documentation.

---

## 📬 Contact

For questions or support, reach out to:

- Pasindu Chandrasiri 
- ✉️ pasinduchandrasiri493@gmail.com  
- 🔗 [GitHub Profile](https://github.com/PasinduChandrasiri)

---

## 🙏 Acknowledgements

Thanks to the n8n community and open-source contributors for making this project possible! 🌟
