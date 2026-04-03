# Nile-University-Midterm-Schedule
# 📅 Exam Schedule Lookup

> A lightweight static web app to find your university exam schedule — instantly.

![Live](https://img.shields.io/badge/status-live-brightgreen)
![Python](https://img.shields.io/badge/python-3.x-blue)
![Hosted on GitHub Pages](https://img.shields.io/badge/hosted-GitHub%20Pages-purple)
![Free](https://img.shields.io/badge/cost-free-lightgrey)

---

## 🧠 The Problem

The university publishes exam schedules as a shared Excel file — inconvenient, hard to navigate, and often inaccessible on mobile. Students had to scroll through hundreds of rows just to find their own exams.

---

## 💡 The Solution

A simple static website where students enter their ID and instantly see only *their* exams. No backend. No login. No cost.

Student IDs are hashed before being stored, so no personal data is exposed in the public repository.

---

## ⚙️ How It Works

1. A Python script reads the university Excel file and converts it to JSON
2. Student IDs are hashed before export
3. A static `index.html` loads the JSON and filters by the entered ID
4. The site is hosted for free on GitHub Pages

---

## 🛠 Tech Stack

- Python + pandas
- JSON
- HTML / CSS / JavaScript
- GitHub Pages

---

## 🚀 Run It Locally
```bash
# 1. Install dependencies
pip install pandas openpyxl

# 2. Place your Excel file and run
python convert.py

# 3. Open index.html in your browser
```

---

## 🔒 Privacy

Student IDs are hashed before being written to `data.json`. Raw IDs are never committed to the repository. All filtering happens client-side — no data is sent to any server.

---

## 🤝 Contributing

Got a suggestion or found a bug? Open an issue or submit a pull request — contributions are welcome.

---

*Built in ~1 hour · Hosted on GitHub Pages · Free forever*
