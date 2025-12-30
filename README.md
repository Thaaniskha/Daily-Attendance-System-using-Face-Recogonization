# 📸 Daily Face Recognition Attendance System

A **computer vision–based daily attendance system** that uses **face recognition** to automatically identify individuals and mark their attendance **once per day** using a webcam.

This project goes beyond simple face detection and performs **real identity recognition** with persistent attendance logging.

---

## 🎯 Project Objective

Traditional attendance methods are:
- ❌ Manual and time-consuming  
- ❌ Easy to manipulate  
- ❌ Inefficient for large groups  

This system provides a **touchless, automated, and accurate attendance solution** using facial recognition.

---

## ✨ Key Features

🟢 Real-time face recognition via webcam  
🧠 Identifies *who* the person is (not just detecting faces)  
🗓️ Marks attendance **only once per day per person**  
📁 Stores attendance data in a CSV file  
📷 Uses known face images as reference database  
🚫 Unknown faces are ignored (not marked)  

---

## 🧠 How It Works

1. Load known face images from the `known_faces/` directory  
2. Extract facial encodings using `face_recognition`  
3. Start live webcam feed  
4. Detect and recognize faces in real time  
5. If a known face is detected:
   - ✅ Name is displayed
   - 🗓️ Attendance is marked (only once per day)
6. Attendance is saved to `attendance.csv`

---

## 🎨 Visual Flow

| Face Detected | Status |
|-------------|--------|
| 🟢 Known Face | Attendance Marked |
| 🔴 Unknown Face | Ignored |
| 📅 Already Marked Today | Skipped |

---

## 🛠️ Technologies Used

- **Python**
- **OpenCV**
- **face_recognition**
- **NumPy**
- **Webcam (Live Video Feed)**

---

## 📂 Project Structure

