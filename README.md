# **Scrape Lazada Ratings & Prices**
## 🚩 Overview  
This script automates scraping price, total ratings, and monthly ratings from Lazada product pages across multiple countries.  

### 🔑 Key Features  
- **Automated Data Extraction** – Uses Playwright to navigate Lazada product pages and extract key details.  
- **Multi-Country Support** – Works across different Lazada country domains.  
- **Total & Monthly Ratings** – Captures both total reviews and last month's reviews.  
- **Dynamic Price Extraction** – Extracts and formats the latest product price from Lazada.  
- **Google Sheets Integration** – Automatically stores scraped data into a Google Sheets document.
- 
---

## 🛠 Requirements  
- Python 3.9+  
- Playwright  
- gspread-pandas  
- pandas, numpy  

---

## 🚀 How to Use  

### 1️⃣ Install dependencies  
```bash
pip install pytest-playwright
```

### 2️⃣ Setup Playwright (only needed once)  
```bash
playwright install  
```

### 3️⃣ Start Chrome with remote debugging  

#### **Step 1:**  
```bash
cd %USERPROFILE%\AppData\Local\ms-playwright\chromium-1129\chrome-win  
```

#### **Step 2:**  
```bash
%USERPROFILE%\AppData\Local\ms-playwright\chromium-1129\chrome-win> .\chrome --remote-debugging-port=9222
```  

#### **Step 3:**  
Open the following URL in your Chromium browser:  
```http
http://localhost:9222/json/version
```  
Copy the value of `webSocketDebuggerUrl` and paste it into the `web_socket_path` variable in the script.  

### 4️⃣ Setup Google Service Account  
- Create a Google Service Account.  
- Save the JSON credentials in the following directory:  
  ```
  %USERPROFILE%\AppData\Roaming\gspread_pandas\google_secret.json
  ```

### 5️⃣ Create a Google Spreadsheet  
- Follow this **[Google Sheets Template](https://docs.google.com/spreadsheets/d/1Lc2Oxqc1Pf2aQrVIbzAd3RnlM4ZGUDe-xgFIrDwzZx4/edit?gid=0)** for formatting.  
- Share access to your service account in this spreadsheet.  

### 6️⃣ Configure the Script  
- Input all necessary settings and parameters before execution.  

### 7️⃣ Run the Script  
- Once everything is set up, execute the script, and Playwright will handle the rest! \ud83d\ude80  









 
