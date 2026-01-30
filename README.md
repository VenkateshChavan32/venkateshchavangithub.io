# Venkatesh Chavan

📧 Email: neil009chavan@gmail.com  
📞 Phone: +91-9518778933  
🔗 LinkedIn: https://linkedin.com/in/venkatesh-chavan-2b717721a/

---

## 📌 Profile Summary

Detail-oriented **Data Analyst** with hands-on experience in building interactive dashboards and extracting insights from raw data. Skilled in **Tableau, Power BI, Excel, and Python**, with a strong foundation in data cleaning, transformation, and KPI reporting. Passionate about turning data into actionable business decisions.

---

## 🛠 Technical Skills

### 📊 Data Visualization & BI Tools
- Tableau  
- Power BI  

### 📈 Data Analysis Tools
- Microsoft Excel  
  - Pivot Tables  
  - VLOOKUP / XLOOKUP  
  - Charts & Dashboards  

### 💻 Programming Languages
- Python  
- C  
- C++  

### 🔍 Data Skills
- Data Cleaning  
- Data Transformation  
- Exploratory Data Analysis (EDA)  
- KPI Reporting  

### 🤝 Soft Skills
- Analytical Thinking  
- Problem Solving  
- Attention to Detail  

---

## 📂 Projects

### 📊 Sales Performance Dashboard (Tableau / Power BI)
- Designed interactive dashboards to analyze **sales trends, revenue, and regional performance**  
- Cleaned and prepared raw datasets using Excel  
- Identified **top-performing products** and **underperforming regions**

---
Smart-File-Organizer/
│
├── file_organizer.py
└── README.md
# 📁 Smart File Organizer (Python)

A single-file Python automation script that organizes files in any folder  
(like Downloads) into categorized subfolders automatically.

---

## 🚀 Features
- Automatically sorts files by type (Images, Videos, Documents, etc.)
- Handles duplicate filenames safely
- Cross-platform (Windows, macOS, Linux)
- No external libraries required
- Clean, single-file design (production-style script)

---

## 🧠 Skills Demonstrated
- Python standard library
- File system automation
- Path handling using `pathlib`
- Error handling & safe file operations
- Clean, readable scripting

---

## ▶ How to Run

```bash
python file_organizer.py

import os
import shutil
from pathlib import Path

TARGET_FOLDER = Path.home() / "Downloads"

FILE_TYPES = {
    "Images": [".jpg", ".jpeg", ".png", ".gif", ".webp"],
    "Videos": [".mp4", ".mkv", ".avi", ".mov"],
    "Documents": [".pdf", ".docx", ".txt", ".pptx", ".xlsx"],
    "Archives": [".zip", ".rar", ".7z", ".tar", ".gz"],
    "Programs": [".exe", ".msi"],
    "Music": [".mp3", ".wav", ".flac"]
}

def get_destination_folder(extension):
    for folder, extensions in FILE_TYPES.items():
        if extension in extensions:
            return folder
    return "Others"

def move_file(file_path):
    ext = file_path.suffix.lower()
    folder_name = get_destination_folder(ext)
    destination_dir = TARGET_FOLDER / folder_name
    destination_dir.mkdir(exist_ok=True)

    destination_path = destination_dir / file_path.name
    counter = 1

    while destination_path.exists():
        destination_path = destination_dir / f"{file_path.stem}_{counter}{ext}"
        counter += 1

    shutil.move(str(file_path), str(destination_path))

def organize_files():
    for item in TARGET_FOLDER.iterdir():
        if item.is_file():
            try:
                move_file(item)
            except Exception as e:
                print(f"Error moving {item.name}: {e}")

    print("✅ Files organized successfully.")

if __name__ == "__main__":
    organize_files()


### 🐍 Data Analysis Using Python
- Performed data cleaning and analysis using **Pandas** and **NumPy**  
- Conducted **Exploratory Data Analysis (EDA)** to identify trends and patterns  
- Visualized insights to support data-driven decision-making  

---

### 📑 Excel Dashboard Project
- Built dynamic dashboards using **Pivot Tables and charts**  
- Automated calculations and **KPI tracking** using formulas  

---

## 🎓 Education

**Master of Computer Applications (M.C.A)**  
📅 2024 – 2026  
🏫 Bharati Vidyapeeth  

**Bachelor of Commerce (B.Com)**  
📅 2021 – 2024  
🏫 Vivekanand College  

---

## 📜 Certifications
- Tableau / Power BI Certification *(if applicable)*  
- Python for Data Analysis *(if applicable)*  

---

## 🚀 Career Interests
- Entry-level **Data Analyst** / **BI Analyst** roles  
- Data-driven problem solving  
- Dashboarding & business insights  

---

## 📎 Notes
This repository serves as a professional overview of my skills, projects, and background in data analytics.  
Feel free to connect with me on LinkedIn or reach out via email.
