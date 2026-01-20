<div align="center">

# 🏠 Data Entry Automation  
### Scrape Zillow-style property listings & auto-fill Google Forms using Python 🚀

<img src="https://readme-typing-svg.demolab.com?font=Poppins&size=24&pause=1000&color=2EA44F&center=true&vCenter=true&width=900&lines=BeautifulSoup+%2B+Requests+%2B+Selenium;Scrape+Property+Data+%F0%9F%8F%A0;Auto-fill+Google+Forms+%F0%9F%93%9D;Save+Responses+in+Google+Sheets+%F0%9F%93%8A" alt="Typing SVG" />

<br>

<p>
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/BeautifulSoup-000000?style=for-the-badge&logo=dependabot&logoColor=white"/>
  <img src="https://img.shields.io/badge/Selenium-43B02A?style=for-the-badge&logo=selenium&logoColor=white"/>
  <img src="https://img.shields.io/badge/Requests-FF6F00?style=for-the-badge&logo=amazonaws&logoColor=white"/>
  <img src="https://img.shields.io/badge/Google%20Forms-673AB7?style=for-the-badge&logo=googleforms&logoColor=white"/>
  <img src="https://img.shields.io/badge/Google%20Sheets-34A853?style=for-the-badge&logo=googlesheets&logoColor=white"/>
</p>

<img src="https://user-images.githubusercontent.com/74038190/216655883-62ab7f1e-8c4f-4d8c-9f6f-90c1d9b5d573.gif" width="520"/>

</div>

---

## ✨ Project Overview

This automation project **scrapes property listings** (Address, Price & Link) from a Zillow-clone website and then **automatically fills a Google Form** using Selenium.

✅ Scrapes from:  
🔗 https://appbrewery.github.io/Zillow-Clone/

✅ Auto fills Google Form fields:
- Address *(short answer)*
- Price *(short answer)*
- Link *(short answer)*

✅ Output:  
📊 Data is stored and presented inside **Google Sheets** *(Google Form responses)*

---

## 🧠 Libraries Used

- **BeautifulSoup4 (bs4)** → HTML parsing & extraction
- **Requests** → Fetching website HTML
- **Selenium WebDriver** → Automating Google Form filling
- **time** → wait / delay for stable page interaction

---

## ⚙️ Workflow

```mermaid
flowchart LR
A[Requests fetch HTML] --> B[BeautifulSoup parses page]
B --> C[Extract Addresses]
B --> D[Extract Prices]
B --> E[Extract Links]
C --> F[Selenium opens Google Form]
D --> F
E --> F
F --> G[Submit Form]
G --> H[Google Sheets Responses]
