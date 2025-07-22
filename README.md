Here's the `README.md` file for my Face Recognition Attendance System GitHub repository:

---

# 🧠 Face Recognition-Based Attendance System 🎓

This project is a **Flask-based web application** that uses **Face Recognition**, **MTCNN**, and **OpenCV** to automate attendance tracking through facial identification. Users (admin/staff) can upload a group photo, and the app will detect known faces and mark attendance accordingly.

---

## 📸 Features

* 👥 Detects multiple faces in group images
* 🔐 Login system for authorized access
* 📁 Upload group images for real-time attendance
* ✅ Marks attendance as *Present* or *Absent*
* 🗓️ Generates timestamped attendance records
* 📊 View total attendance summary for each student
* 📤 Download full attendance report as CSV
* 🧾 View registered students and their images

---

## 🛠️ Tech Stack

* **Frontend:** HTML, CSS, Flask
* **Backend:** Python (Flask)
* **Face Detection:** MTCNN
* **Face Recognition:** `face_recognition` library
* **Data Handling:** Pandas, CSV
* **Image Processing:** OpenCV

---

## 📂 Folder Structure

```
.
├── static/
│   ├── data/              # Training images organized by student name
│   ├── result.jpg         # Annotated result image
│   └── uploads/           # Uploaded group images
├── templates/             # HTML templates
├── users.csv              # Login credentials
├── data.csv               # Attendance record
├── app.py                 # Main Flask application
└── README.md              # Project documentation
```

---

## 🧪 Setup Instructions

1. **Clone the repository**

```bash
git clone https://github.com/yourusername/face-attendance-system.git
cd face-attendance-system
```

2. **Create a virtual environment**

```bash
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows
```

3. **Install dependencies**

```bash
pip install -r requirements.txt
```

> Example `requirements.txt`:

```txt
flask
face_recognition
opencv-python
numpy
pandas
mtcnn
```

4. **Add training images**

   * Place student images under `static/data/<Student_Name>/`
   * Each student's folder can have multiple images.

5. **Create a login user**

   * Create `users.csv` with the following format:

     ```
     username,password
     admin,admin123
     ```

6. **Run the application**

```bash
python app.py
```

7. **Access in browser**

```
http://localhost:5050
```

---

## 📌 Screenshots

> *(Add your own screenshots here for `login`, `dashboard`, `attendance summary`, etc.)*

---

## 📈 Sample Workflow

1. Log in with valid credentials.
2. Upload a group photo via dashboard.
3. System processes and marks recognized students as **Present**.
4. Result image is shown with recognized names.
5. View detailed attendance or download report.

---

## 📥 Download Attendance

Go to `/download_attendance_csv` to download the complete CSV file with timestamped records.

---

## ✅ Future Improvements

* Add face registration from UI
* Real-time webcam integration
* Admin/user role separation
* Email/SMS notifications

---

## 👨‍💻 Author

**Abhik Roy Chowdhury**

---
