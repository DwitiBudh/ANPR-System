# Smart ANPR System for Gated Communities 🚗

An **AI-powered Automatic Number Plate Recognition (ANPR) system** designed for gated communities and parking areas.
The system automatically detects vehicle number plates, reads the plate number, verifies it with a database, and logs entry or exit events in real time.

This project uses **YOLOv8 for number plate detection**, **EasyOCR for character recognition**, and **Flask for building the web interface and API**.

---

# 📌 Project Overview

Manual vehicle entry systems used in many gated communities are slow and prone to errors. Security guards often record vehicle numbers manually, which can lead to long queues and inaccurate logs.

The **Smart ANPR System** solves this problem by automating the entire process.

The system can:

* Detect number plates from camera input
* Read the plate characters using OCR
* Verify vehicles using a database
* Allow or deny entry automatically
* Maintain a digital record of all vehicles
* Provide analytics through a dashboard

---

# ⚙️ System Workflow

The project follows a simple pipeline:

1. **Capture Image**

   * Image is captured from a live camera or uploaded manually.

2. **Plate Detection**

   * YOLOv8 detects the number plate region in the image.

3. **Plate Cropping**

   * The detected number plate area is cropped.

4. **OCR Recognition**

   * EasyOCR reads the characters on the plate.

5. **Database Verification**

   * The system checks whether the vehicle is registered or blacklisted.

6. **Decision**

   * The system allows or denies entry and logs the event.

---

# 🚀 Key Features

* **Real-Time Number Plate Detection**
* **Automatic Vehicle Entry and Exit Logging**
* **OCR-Based Plate Recognition**
* **Night Mode Image Enhancement**
* **Multi-Camera Support**
* **Vehicle Type Detection (Car / SUV / Bike / Truck)**
* **Speed Estimation and Overspeed Alerts**
* **Analytics Dashboard for Traffic Insights**
* **Secure Database Logging**

---

# 🧠 Technologies Used

### Computer Vision & AI

* YOLOv8 (Ultralytics)
* EasyOCR
* OpenCV
* NumPy

### Backend

* Python
* Flask
* SQLite Database
* Threading

### Frontend

* HTML
* CSS
* JavaScript

### Image Processing

* CLAHE (Contrast Enhancement)
* Gamma Correction
* Bilateral Filtering
* Unsharp Masking

---

# 📊 Performance

| Metric                     | Value       |
| -------------------------- | ----------- |
| Plate Detection Accuracy   | ~95%        |
| OCR Accuracy               | ~88%        |
| End-to-End Processing Time | < 2 seconds |
| Live Stream Frame Rate     | ~25 FPS     |

---

# 📂 Project Structure

```
ANPR-System
│
├── app.py
├── detection.py
├── ocr.py
├── analytics.py
├── database.db
│
├── static
│   ├── css
│   ├── js
│   └── images
│
├── templates
│   ├── index.html
│   ├── dashboard.html
│
├── models
│   └── yolov8_weights.pt
│
└── README.md
```

---

# 🖥️ Installation

Clone the repository:

```
git clone https://github.com/yourusername/anpr-system.git
```

Move into the project directory:

```
cd anpr-system
```

Install dependencies:

```
pip install -r requirements.txt
```

Run the application:

```
python app.py
```

The system will start a local Flask server and open the dashboard.

---

# 📸 Example Output

The system detects a vehicle plate and returns:

```
Plate Number: GJ01AB1234
Status: Allowed
Confidence: 92%
Time: 10:42 AM
```

All results are stored in the database and shown in the analytics dashboard.

---

# 📈 Analytics Dashboard

The system dashboard provides insights such as:

* Hourly traffic heatmap
* Entry vs exit statistics
* OCR confidence distribution
* Vehicle speed analytics
* Anomaly detection alerts

These analytics help management understand traffic patterns and improve security.

---

# 🔮 Future Improvements

* Mobile application for guards
* Cloud-based centralized dashboard
* Automatic barrier gate integration
* WhatsApp visitor verification
* Face recognition for pedestrian entry
* RFID + ANPR hybrid verification
* GPU optimization for faster inference

---

# 👥 Team

**Team 11 – PGDM Artificial Intelligence & Data Science**

* Srashti Soni
* Dwiti Budh
* Digesh Patel
* Ravindra Tanwar
* Priya A

---

# 📜 License

This project is created for **academic and research purposes**.
Feel free to modify and extend the project for learning and experimentation.

---



