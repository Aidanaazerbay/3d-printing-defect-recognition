# 3D Printing Defect Recognition System (YOLOv8 + Computer Vision)
Developed by team **"Young Engineers"** (*"Молодые инженеры"*) during the **Cosmothon Hackathon** (organized by SEDS KZ at Nazarbayev University).
This project focuses on automated computer vision-based flaw detection during the 3D printing process to minimize material waste and improve manufacturing efficiency.
## Key Capabilities & Architecture
### 1. Computer Vision Pipeline (YOLOv8)
**Real-time Flaw Detection:** Detects defects (e.g., Z-seam, pillowing, spaghetti, plastic finish, and retraction flaws) directly on 3D printed objects.
**Model Training & Confusion Matrix:** Trained on custom datasets with high accuracy, low false-positive rates, and proven convergence metrics.
### 2. System Architecture & Flowchart
**Image Capture:** Camera attached to the 3D printer sends HTTP POST requests with capture images.
**API Server:** Flask backend validates requests and runs inferences using trained YOLOv8 weights.
**Annotated Output:** Returns bounding box coordinates (`bboxes`) and annotated images encoded in base64/JSON to alert operators in real-time.
## Economic Impact & Cost Savings
**Material Waste Reduction:** Early defect identification prevents scrapping entire prints midway.
**Production Efficiency:** Reduces human inspection time and overall machine downtime.
**Throughput Increase:** Enables automated 24/7 quality assurance for industrial 3D printing.
## Tech Stack
**Computer Vision / AI:** YOLOv8, PyTorch, OpenCV
**Backend:** Flask (Python)
**Design & Presentation:** Canva, Data Visualization
