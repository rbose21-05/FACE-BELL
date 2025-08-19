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
