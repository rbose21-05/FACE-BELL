# FACE-BELL 🔔

A face recognition doorbell system using React and Flask with DeepFace AI.

## Features

- Real-time face recognition using webcam
- Add new faces to the database
- Visitor logging system
- Audio alerts for recognized/unrecognized faces

## Prerequisites

- Python 3.9+
- Node.js 16+
- npm or yarn
- Webcam access

## Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/rbose21-05/FACE-BELL.git
cd FACE-BELL
```

### 2. Backend Setup
```bash
cd backend

# Install Python dependencies
pip3 install -r requirements.txt

# Create faces directory (if it doesn't exist)
mkdir -p faces

# Start the Flask server
python3 app.py
```

The backend will run on `http://127.0.0.1:5000`

### 3. Frontend Setup

Open a new terminal window:
```bash
cd frontend/my-project

# Install dependencies
npm install

# Start the development server
npm run dev
```

The frontend will run on `http://localhost:5173`

### 4. macOS Users: Disable AirPlay Receiver

If you get a "Port 5000 is in use" error:

1. Open **System Settings**
2. Go to **General** → **AirDrop & Handoff**
3. Turn OFF **AirPlay Receiver**

## Usage

1. Open `http://localhost:5173` in your browser
2. Allow webcam access when prompted
3. Click **"📸 Capture Face"** to recognize a face
4. If face is not recognized, you can add it to the database
5. Click **"📄 View Visitor Log"** to see visitor history

## Project Structure
```
FACE-BELL/
├── backend/
│   ├── app.py              # Flask API server
│   ├── requirements.txt    # Python dependencies
│   ├── faces/             # Face database directory
│   └── visitor_log.csv    # Visitor log file
├── frontend/
│   └── my-project/
│       ├── src/
│       │   ├── App.jsx           # Main React component
│       │   ├── VisitorLog.jsx    # Visitor log component
│       │   └── main.jsx
│       ├── public/
│       │   ├── bell.mp3          # Recognition sound
│       │   └── alarm.mp3         # Alert sound
│       ├── vite.config.js        # Vite proxy configuration
│       └── package.json
└── README.md
```

## Technologies Used

### Backend
- Flask - Web framework
- DeepFace - Face recognition AI
- OpenCV - Image processing
- Flask-CORS - Cross-origin resource sharing

### Frontend
- React - UI framework
- Vite - Build tool and dev server
- Axios - HTTP client
- Framer Motion - Animations
- React Webcam - Camera access

## API Endpoints

- `POST /recognize` - Recognize a face from base64 image
- `POST /add_face` - Add a new face to the database
- `POST /log` - Get visitor log (requires key: "211005")
- `POST /clear_log` - Clear the visitor log

## Troubleshooting

### CORS Issues
This project uses Vite's proxy feature to avoid CORS issues in development. The proxy is configured in `vite.config.js` to forward `/api/*` requests to the Flask backend.

### Face Recognition Not Working
- Ensure the `faces` folder exists in the backend directory
- Make sure there's adequate lighting for the webcam
- Check that DeepFace dependencies are properly installed

### Port Conflicts
- Backend uses port 5000 (may conflict with macOS AirPlay)
- Frontend uses port 5173 (Vite default)

## License

MIT

## Contributors

- Rupsa Bose (rbose21-05)
