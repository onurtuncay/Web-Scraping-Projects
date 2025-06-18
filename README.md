# 🛍️ Koton Web Scraper

**Author:** Onur Tuncay

This project is a simple Python script designed to scrape product information from [koton.com](https://www.koton.com), a popular fashion e-commerce website. It uses `requests` and `BeautifulSoup` to collect and structure the data, which is then stored in a pandas DataFrame for further use or export.

## 📦 What It Does

- Sends HTTP requests to a Koton category or search page.
- Extracts product-level data such as:
  - Product Name
  - Product Price
  - Product Link
- Stores the collected information in a structured DataFrame.
- Can be extended to save data as `.csv`, analyze prices, track changes, or feed into a larger pipeline.

## ⚠️ About the User-Agent

To avoid being blocked by the website, the script requires a **User-Agent** string in the request headers.

🔐 **How to get your User-Agent:**
1. Open [https://www.whatismybrowser.com/](https://www.whatismybrowser.com/)
2. Copy your browser's full User-Agent string.
3. Replace this line in the code:

```python
headers = {"User-Agent": "your_user_agent"}
headers = {"User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64)..."}  # Your string here
```
## 🛠️ Requirements
Install the required packages using:

```bash
pip install -r requirements.txt
```

## 🚀 How to Run
Make sure the script or notebook (KotonWebScraping.ipynb) is in your working directory, then run the cells step by step in a Jupyter Notebook environment, or convert it into a .py file and run:

```bash
python koton_scraper.py
```

## 📌 Disclaimer
This project is for educational purposes only. Please check the website’s robots.txt and terms of service before using this script extensively.


