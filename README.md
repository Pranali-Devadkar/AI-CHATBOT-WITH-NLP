# AI-CHATBOT-WITH-NLP

COMPANY: CODTECH IT SOLUTIONS

NAME: DEVADKAR PRANALI HANUMANT

INTERN ID: CT06DG1339

DOMAIN: PYTHON PROGRAMMING

DURATION: 6 WEEKS

MENTOR: NEELA SANTHOSH

📊 Automated Report Generation

This project is a simple Python script that reads student names and scores, analyzes the data, and generates a formatted PDF report. It demonstrates how to automate report creation using the reportlab library in Python.

---

## 🚀 Features

- Reads data (student names and scores)
- Calculates average score
- Generates a clean, formatted PDF report
- Easy to run on mobile using *Pydroid 3* or any Python IDE

---

## 🧰 Tools & Technologies

| Tool        | Description                            |
|-------------|----------------------------------------|
| Python      | Programming language                   |
| ReportLab   | Library for generating PDF documents   |
| Pydroid 3   | Android-based Python IDE (for testing) |
| GitHub      | Version control and code hosting       |

---

## 📁 Project Structure

automated-report/ │ ├── simple_report.pdf      # Output PDF file ├── report_generator.py    # Main Python script ├── README.md              # Project documentation

---

## 🧾 Sample Output (PDF Report)

*Report Title:* Student Scores Report  
*Details:*

Ali: 85
Sara: 90
Ahmed: 78
Noor: 88

Average Score: 85.25

---

## 📜 Python Script Overview

```python
from reportlab.pdfgen import canvas
import os

# Data
names = ["Ali", "Sara", "Ahmed", "Noor"]
scores = [85, 90, 78, 88]
average = sum(scores) / len(scores)

# Output PDF path
file_name = "simple_report.pdf"
file_path = os.path.join(os.getcwd(), file_name)

# PDF generation
c = canvas.Canvas(file_path)
c.drawString(100, 800, "Student Scores Report")
y = 770

for i in range(len(names)):
    line = f"{names[i]}: {scores[i]}"
    c.drawString(100, y, line)
    y -= 20

c.drawString(100, y - 20, f"Average Score: {average:.2f}")
c.save()

print(f"PDF created: {file_path}")


---

📦 Requirements

Install the ReportLab library using pip:

pip install reportlab

Or install from Pydroid 3 > Pip menu (if using Android).


---

💡 How to Run

1. Install Python or use Pydroid 3 (for mobile).


2. Copy the script into a .py file (e.g., report_generator.py).


3. Run the script.


4. Check the current directory for the generated simple_report.pdf.




---

📬 Deliverables

✅ Python script (report_generator.py)

✅ Sample report PDF (simple_report.pdf)



---

📌 Author

Pranali Devadkar
GitHub Profile



#OUTPUT

