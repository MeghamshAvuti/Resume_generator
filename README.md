# 📄 Resume Generator 

## Project Overview
This is a resume generator application that takes details from the user through a form, generates a resume in PDF format, and stores data in a backend database (MySQL/MongoDB). The application incorporates the IPStack API to automatically fetch the user's geolocation.

##  Features
 **Dynamic Resume Form**: Users can enter personal details, work experience, skills, and projects.  
 **Geolocation Tracking**: Automatically detects and fills in the user's **City, Region, and Country**.  
 **Resume Templates**: Users can choose from **three resume templates**.  
 **PDF Resume Generation**: Converts the resume into a **downloadable PDF** using **WeasyPrint**.  
 **Database Storage**: Saves user resume details in **MySQL/MongoDB**.  
 **RESTful API**: Built with **FastAPI**, providing endpoints for form submission, PDF generation, and fetching location.

---

## 🛠 Tech Stack
**Frontend:**  
- HTML, CSS (Tailwind/Bootstrap)  
- JavaScript (Fetch API for backend communication)

**Backend:**  
- **FastAPI (Python)**  
- **MySQL / MongoDB** (Choose one)  
- **WeasyPrint** (For PDF Generation)  
- **IPStack API** (For Geolocation)

---

## 📥 Installation Guide

### 🔹 Step 1: Clone the Repository

git clone  https://github.com/MeghamshAvuti/Resume_generator
cd resume-generator

Step 2: Set Up Virtual Environment
python -m venv venv

Windows
venv\Scripts\activate

Mac/Linux
source venv/bin/activate

Step 3: Install Dependencies
pip install -r requirements.txt

Step 4: Configure Database (MySQL)
CREATE DATABASE resumes_db;

Update database.py with your database credentials:
DATABASE_URL = "mysql+pymysql://root:password@localhost/resumes_db"

Running the Application
1️⃣ Start the Backend Server
Run the FastAPI server:
uvicorn main:app --reload

🌍 Frontend Usage
1️⃣ Open frontend/index.html in a browser
2️⃣ Fill in the resume form
3️⃣ Click Generate Resume
4️⃣ Download the PDF resume

🚀 Deployment Guide (Optional)
🔹 Deploy Backend on Render
Create a new Render web service
Connect your GitHub repo
Set up a PostgreSQL or MongoDB instance
Deploy with Gunicorn:

🔹 Deploy Frontend on Netlify/Vercel
Upload the frontend folder
Deploy and get a Live Link

🛠 Troubleshooting
❌ Database Connection Error?

Ensure MySQL/MongoDB is running
Check DATABASE_URL in database.py
❌ PDF Not Generating?

Check if WeasyPrint is installed
Try: pip install weasyprint
📌 Future Enhancements
⭐ User Authentication (Login/Signup)
⭐ More Resume Templates
⭐ Resume Editing Feature

🤝 Contributing
1️⃣ Fork the repository
2️⃣ Create a new branch:
git checkout -b feature-name
git commit -m "Added new feature"
4️⃣ Push to GitHub & create a Pull Request.

📞 Contact
✉️ Your Name - Meghamsh Avuti
📌 GitHub: https://github.com/MeghamshAvuti
📌 LinkedIn: https://www.linkedin.com/in/avutimeghamsh/

