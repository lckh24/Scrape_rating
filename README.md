# Scrape Lazada Ratings & Prices

## 📌 Overview  
This script automates scraping price, total ratings, and monthly ratings from Lazada product pages across multiple countries.  
🛠️ Key Features  
* Automated Data Extraction – Uses Playwright to navigate Lazada product pages and extract key details.  
* Multi-Country Support – Works across different Lazada country domains.  
* Total & Monthly Ratings – Captures both total reviews and last month's reviews.   
* Dynamic Price Extraction – Extracts and formats the latest product price from Lazada.  
* Google Sheets Integration – Automatically stores scraped data into a Google Sheets document.  
* Sorting & Filtering – Allows sorting reviews by criteria like "most recent" for better insights.  
* Fuzzy Matching for URLs – Ensures the correct product page is selected by comparing URL similarity.  
* Error Handling & Logging – Implements error handling to ensure smooth execution and logs potential failures.  
🔧 Requirements
Python 3.9+  
Playwright   
gspread-pandas   
pandas, numpy   
🚀 How to Use  
1️⃣ Install dependencies  
2️⃣ Setup Playwright (only needed once)
  ``` bash
  pip install pytest-playwright
  ```  
  ``` bash
  playwright install  
  ```
  
3️⃣ Start Chrome with remote debugging  
Step 1:   
```bash
 cd %USERPROFILE%\AppData\Local\ms-playwright\chromium-1129\chrome-win  
```
Step 2:  
``` bash
%USERPROFILE%\AppData\Local\ms-playwright\chromium-1129\chrome-win>  .\chrome --remote-debugging-port=9222
```
Step 3:
Search ```http://localhost:9222/json/version``` in chromium browser and copy the value of webSocketDebuggerUrl => Paste the value in  ```web_socket_path``` variable  
Step 4:  
Input all information  
Step 5:
Starting the code










 
