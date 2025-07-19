# 🛒 Amazon Screenshot Bot

A Python desktop tool that automates taking **screenshots** of Amazon.in search results based on keywords from a CSV or Excel file.

---

## 📸 Features

✅ Simple UI for uploading and running  
✅ Supports `.csv`, `.xlsx` files (no headers required)   
✅ Ensure Top of Search
✅ Automatically saves screenshots in a timestamped folder  
✅ Handles CAPTCHA with retry logic  
✅ Logs failed keywords in Excel  
✅ Generates a summary CSV of success/failure  

---

## 📁 Output Structure

Added functionality to choose the destination folder for saving files. Files are saved in the selected path with a timestamped folder name (e.g., D:\amazon_ss\<timestamp>).

```
📂 D:\amazon_ss\2025-06-24_21-37-12\
├── yoga_mat.png
├── dumbbell_set.png
├── summary.csv              # keyword, status, filename, notes
└── failed_keywords.xlsx     # only keywords that failed
```

---

## 🚀 How to Run (Step-by-Step)

### 🛠️ Prerequisites

- ✅ Windows with **Python 3.8+**
- ✅ Google Chrome installed
- ✅ `pip` available (comes with Python)

---

### 📁 1. Download and Extract the Project

If you received a ZIP:
- Extract it to any folder (e.g., `C:\amazon-screenshot`)

Or if using Git:
```bash
git clone https://github.com/MUKUNDSINGHKUSHWAHA/amazon-screenshot-bot.git
cd amazon-screenshot-bot
```

---

### 📦 2. Install Required Libraries

Open **Command Prompt** or **PowerShell**, navigate to the project folder, and run:

```bash
pip install -r requirements.txt
```

This will install:
- `selenium`
- `pandas`
- `openpyxl`
- `pillow`
- `undetected-chromedriver`

---

### ▶️ 3. Run the App

In the same terminal, run:

```bash
python main.py
```

This will launch a simple desktop UI window.

---

### 📂 4. Use the Tool

1. Click **Browse** and select your `.csv` or `.xlsx` file  
   - Ensure search terms are in **Column A**, no header needed  
2. Click **Start**  
3. Wait for the **“Completed”** popup  
4. Check your screenshots and reports in:  
   ```
   D:\amazon_ss\<date_time>\
   ```

---

 
