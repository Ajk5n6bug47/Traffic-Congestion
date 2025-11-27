# 🚔 Traffic Incident Test Report System  
Comprehensive Reporting for PSV Drivers, Police Incidents, and Theft Cases in Nairobi

---

## 📌 Overview  
The **Traffic Incident Test Report System** is a data processing and reporting tool designed to manage, analyze, and generate structured reports for:

- PSV driver tests  
- Police officer assessments  
- Theft and criminal incident evaluations  

The system simulates **real Nairobi incident locations**, realistic timestamps, officer IDs, GPS coordinates, severity levels, vehicle plates, and outcome results (Passed / Failed / Suspect).

It is ideal for:
- Law-enforcement reporting  
- PSV compliance testing  
- Data analysis  
- Dashboard integration  
- Record keeping  

---

## ✨ Features  
- ✔️ 42+ realistic test entries (PSV, Police, Theft)  
- ✔️ Nairobi-specific locations (CBD, Westlands, Kasarani, Embakasi, etc.)  
- ✔️ GPS coordinates for each incident  
- ✔️ Severity classification (Low/Med/High)  
- ✔️ Officer and driver ID tracking  
- ✔️ Incident categories: Theft, PSV Check, Police Test  
- ✔️ Accurate timestamp generation  
- ✔️ Vehicle plate number assignment  
- ✔️ Final test outcome (Pass / Fail / Suspect)  
- ✔️ Spreadsheet (Excel/CSV) compatible  
- ✔️ Ready for MySQL, dashboards, or reporting systems  

---

## 📁 Project Structure  
```
traffic-incident-system/
│── data/
│   ├── incident_test_data.xlsx
│   ├── incident_test_data.csv
│── src/
│   ├── main.py
│   ├── db_connect.py
│   ├── report_generator.py
│── README.md
│── requirements.txt
```

---

## 🛠 Installation  

Clone the repository:

```bash
git clone https://github.com/yourname/traffic-incident-system.git
cd traffic-incident-system
```

Install Python dependencies:

```bash
pip install -r requirements.txt
```

---

## ▶️ Usage  

### **Run the data processor**
```bash
python main.py
```

### **Load dataset in Python**
```python
import pandas as pd
df = pd.read_excel("data/incident_test_data.xlsx")
print(df.head())
```

---

## 📊 Dataset Columns  

| Column | Description |
|--------|------------|
| Case_Number | Unique incident case number |
| Officer_ID | Officer handling the incident |
| Driver_ID | PSV driver ID (if applicable) |
| Vehicle_Plate | PSV vehicle plate |
| Incident_Type | Theft / PSV Check / Police Test |
| Outcome | Pass / Fail / Suspect |
| Location_Name | Nairobi location |
| GPS_Lat | Latitude |
| GPS_Long | Longitude |
| Severity | Low / Medium / High |
| Timestamp | Time of incident |
| Notes | Extra observations |

---

## 🧭 Supported Nairobi Locations  
Examples:  
- Westlands  
- CBD Nairobi  
- Kasarani  
- Embakasi  
- South B  
- Rongai  
- Kariobangi  
- Industrial Area  
- Pangani  
- Parklands  

---

## 🧰 Technology Stack  
- Python 3.10+  
- Pandas  
- OpenPyXL / CSV  
- MySQL (optional)  
- Git & GitHub  
- ReportLab (optional PDF export)  
- Flask / Streamlit (optional dashboard)  

---

## 🗄️ MySQL Integration  
Your system supports MySQL insertions via:

```python
import mysql.connector

connection = mysql.connector.connect(
    host="your_mysql_host",
    user="your_mysql_user",
    password="your_password",
    database="your_database"
)
```

Tables can store:
- Driver details  
- Officer details  
- Incident logs  
- Test results  

---

## 🚀 Future Enhancements  
- Live dashboard (Streamlit / Flask)  
- Automated PDF reports  
- GPS heatmap visualizations  
- SMS/Email notifications  
- Crime trend analytics  
- Facial recognition integration (optional)

---

## 👤 Author  
**Your Name**  
GitHub: *your github link*  
Email: *your email*

---

## 🙏 Acknowledgements  
Thanks to Nairobi security analysts and PSV compliance officers for contributing realistic scenario data.

---

