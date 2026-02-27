# 🏙️  AI-Powered Smart Urban System

An AI-powered Smart Grievance Management Platform that enables citizens to report waste management issue with image and location support while helping municipal authorities intelligently prioritize complaints using clustering, heatmaps, and AI validation.

---

## 🚀 Problem Statement

Municipal corporations receive thousands of complaints daily.

Current systems:
- Generate duplicate tickets
- Lack intelligent prioritization
- Do not validate complaint authenticity
- Provide limited analytics for decision-making

This leads to delayed resolutions and inefficient resource allocation.

---

## 💡 Our Solution

We developed a full-stack AI-powered complaint management system that:

- 📍 Collects geotagged complaints
- 🖼 Validates uploaded images using YOLO object detection
- 🧠 Detects duplicate complaints using DBSCAN clustering
- 🔥 Generates heatmaps to identify high-density problem zones
- 📊 Helps authorities prioritize based on severity and density

---

## 🛠️ Tech Stack

### Frontend
- React (Vite)
- Axios
- Leaflet (Map Visualization)

### Backend
- FastAPI
- Uvicorn
- Python

### AI / ML
- YOLO (Object Detection)
- DBSCAN (Density-Based Clustering)
- Heatmap Analytics

### Database
- MongoDB (NoSQL, Document-Based Storage)
- Motor / PyMongo (MongoDB driver for FastAPI)

---

## 🧠 Why MongoDB?

We use MongoDB because:

- Flexible document schema for complaint data
- Efficient storage of nested JSON (location + metadata)
- Scalable for large urban datasets
- Geospatial indexing support for location-based queries
- Better suited for real-time analytics and clustering

---

## 📂 Project Structure

Hackathon/
│
├── hackathon-frontend/
│   ├── src/
│   ├── Home.jsx
│   └── package.json
│
├── hackathon-backend/
│   ├── main.py
│   ├── models/
│   ├── database.py
│   ├── requirements.txt
│   └── venv/

---

## ⚙️ Installation & Setup

### 1️⃣ Clone Repository

```bash
git clone https://github.com/yourusername/your-repo-name.git
cd Hackathon

## 2️⃣ Backend Setup (FastAPI + MongoDB)

```bash
cd hackathon-backend
python -m venv venv
venv\Scripts\activate   # Windows
pip install -r requirements.txt


#Make sure MongoDB is running locally:

mongod

Then start the backend:

uvicorn main:app --reload

#Backend runs at:

http://127.0.0.1:8000
3️⃣ Frontend Setup (React)
cd hackathon-frontend
npm install
npm run dev

#Frontend runs at:

http://localhost:5173
##🔐 CORS Configuration

CORS is enabled in FastAPI to allow secure communication between:

React Frontend (Port 5173)

FastAPI Backend (Port 8000)

##📊 Core Features

✅ AI-powered image validation

✅ Geospatial duplicate detection (DBSCAN)

✅ Heatmap visualization

✅ Smart complaint prioritization

✅ MongoDB geospatial indexing

✅ Scalable architecture

##🧠 AI Pipeline

User uploads complaint (text + image + location)

YOLO validates image object

Complaint stored in MongoDB

DBSCAN clusters nearby complaints

Heatmap generated for authority dashboard

Priority score assigned

##🎯 Use Cases

Smart Cities

Municipal Corporations

Waste Management

Infrastructure Monitoring

Urban Planning Analytics

##📈 Future Enhancements

Citizen credibility scoring

Predictive complaint forecasting

Real-time dashboard for administrators

Multi-language NLP support

Cloud deployment (AWS / Azure)

Microservices architecture

##👩‍💻 Team

Built for Hackathon 2026
Team Name:ResponseX
Developed by: Shweta Datey
Archita Raghuvanshi
Pranjal Rane
