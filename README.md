# AI-OBJECT-DETECTION-SYSTEM

A full-stack AI Object Detection System built with React, FastAPI, and YOLOv8. Features real-time live camera detection via WebSockets and video upload processing, all fully containerized with Docker.

## Features
- **Live Camera Detection**: High-speed real-time bounding boxes via WebSockets.
- **Video Upload**: Process MP4 files using YOLO and download webm videos.
- **Dockerized**: Easy setup with Docker Compose.

## How to Run

### Using Docker
```bash
docker-compose up --build
```
- Frontend will be available at `http://localhost:3000`
- Backend will be available at `http://localhost:8000`

### Local Development
**Backend**:
```bash
cd backend
python -m venv venv
source venv/bin/activate  # On Windows: .\venv\Scripts\activate
pip install -r requirements.txt
uvicorn main:app --reload --port 8000
```

**Frontend**:
```bash
cd frontend
npm install
npm run dev
```
