# 📸 FACE_BELL

A **Smart Doorbell System** built with **Flask (Python backend)** and **React (Frontend)**.  
It captures visitor faces 👤, stores them 📂, and shows a **visitor log** with access control 🔐.

---

## 🚀 Features
- 🎥 Capture faces from webcam
- 🤖 Face recognition & storage with DeepFace + OpenCV
- 📑 Visitor log saved in CSV
- 🌐 Modern frontend with React + Vite
- 🔄 Access-controlled log viewing

---

## ⚡ Setup Instructions

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/rbose21-05/FACE_BELL.git
cd FACE_BELL
2️⃣ Start the Backend (Flask + Python)
bash
Copy
Edit
cd backend
python -m venv venv
Activate virtual environment:

Windows

bash
Copy
Edit
venv\Scripts\activate
Mac/Linux

bash
Copy
Edit
source venv/bin/activate
Install dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Run the backend:

bash
Copy
Edit
python app.py
✅ Flask will start at: http://127.0.0.1:5000/

3️⃣ Start the Frontend (React + Vite)
Open a new terminal (keep backend running):

bash
Copy
Edit
cd frontend/my-project
npm install
npm run dev
✅ React will start at: http://localhost:5173/

4️⃣ Usage
Open the frontend in browser 🌐

Capture a face 📸 → Sent to Flask backend

Backend saves face in faces/ & logs entry in visitor_log.csv

View visitor history in Visitor Log page

📂 Project Structure
bash
Copy
Edit
FACE_BELL/
│── backend/
│   ├── app.py
│   ├── faces/             # Saved face images
│   ├── visitor_log.csv    # Visitor logs
│   └── requirements.txt
│
│── frontend/my-project/
│   ├── src/
│   │   ├── App.jsx
│   │   ├── VisitorLog.jsx
│   │   ├── index.css
│   │   └── main.jsx
│   ├── vite.config.js
│   └── package.json
│
└── README.md
🛠️ Tech Stack
Frontend: React, Vite, TailwindCSS (optional styling)

Backend: Flask, Python, Flask-CORS

AI/ML: DeepFace, TensorFlow, OpenCV

Data Storage: CSV (visitor logs), Images (faces/)

🤝 Contributing
Pull requests are welcome! For major changes, please open an issue first to discuss.

📜 License
MIT License © 2025 Rupsa Bose

yaml
Copy
Edit

---

✨ This version adds **icons, sections, clear formatting, and polish**.  
Want me to also make you a **badge section** (Python | Flask | React | Vite | OpenCV badges) at the top for an even cooler look?







You said:
yes


ChatGPT said:
Here’s a much cleaner and professional-looking README.md you can copy-paste directly into your repo 👇

markdown
Copy
Edit
# 📸 FACE_BELL

A **Smart Doorbell System** built with **Flask (Python backend)** and **React (Frontend)**.  
It captures visitor faces, stores them, and displays a **secure visitor log** with access control.  

---

## 🚀 Features
- 🎥 **Face Capture** using webcam  
- 🖼️ Stores visitor images in `faces/` folder  
- 🗂️ Maintains visitor history in `visitor_log.csv`  
- 🔒 Access-controlled **Visitor Log** page  
- ⚡ Fast frontend built with **React + Vite**  

---

## ⚙️ Setup Instructions

### 🔹 1. Clone the Repository
```bash
git clone https://github.com/rbose21-05/FACE_BELL.git
cd FACE_BELL
🔹 2. Start the Backend (Flask + Python)
bash
Copy
Edit
cd backend
python -m venv venv
▶️ Activate Virtual Environment
Windows

bash
Copy
Edit
venv\Scripts\activate
Mac/Linux

bash
Copy
Edit
source venv/bin/activate
📦 Install Dependencies
bash
Copy
Edit
pip install -r requirements.txt
▶️ Run Backend
bash
Copy
Edit
python app.py
✅ Flask will run at: http://127.0.0.1:5000/

🔹 3. Start the Frontend (React + Vite)
(Open a new terminal, keep backend running)

bash
Copy
Edit
cd frontend/my-project
npm install
npm run dev
✅ React will run at: http://localhost:5173/

🖥️ Usage
Open frontend in browser.

Capture a visitor face → Sent to Flask backend.

Backend saves face in faces/ folder & logs details in visitor_log.csv.

View visitor history in Visitor Log page.

📂 Project Structure
bash
Copy
Edit
FACE_BELL/
│── backend/
│   ├── app.py
│   ├── faces/             # Saved visitor face images
│   ├── visitor_log.csv    # Visitor logs
│   └── requirements.txt
│
│── frontend/my-project/
│   ├── src/
│   │   ├── App.jsx
│   │   ├── VisitorLog.jsx
│   │   ├── index.css
│   │   └── main.jsx
│   ├── vite.config.js
│   └── package.json
│
└── README.md
🤝 Contributing
Pull requests are welcome! For major changes, please open an issue first to discuss.
