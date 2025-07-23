# 🩺 Smart-Nutri

**Smart-Nutri** is a full-stack medical appointment management system that allows users to track their past and upcoming medical visits with ease. Built using Django REST Framework and React.js (Vite), it offers authentication, filtering, and responsive design for a seamless user experience.

## 📌 Project Overview

Smart-Nutri is designed to help users manage their personal medical appointments. It provides full CRUD functionality, user-specific authentication, filtering by status/date, and real-time appointment summaries — all in a clean, responsive interface.

## ✨ Features

- 🔐 **JWT Authentication** – Secure login & signup  
- 🗂 **CRUD Operations** – Create, read, update, delete appointments  
- 📅 **Filtering & Sorting** – Filter appointments by status/date range, sort by date  
- 📊 **Summary View** – Displays total appointments and counts by status  
- 📱 **Responsive UI** – Mobile-friendly with Tailwind CSS  
- 🌐 **RESTful API** – Built with Django REST Framework  


## 🛠 Tech Stack

### 🧩 Frontend
- React.js (Vite)  
- Tailwind CSS  
- Axios  
- React Router DOM  

### 🔧 Backend
- Django  
- Django REST Framework  
- SimpleJWT (Authentication)  
- PostgreSQL  

  

## 📥 Installation Instructions

### 1. **Clone the Repository**
```bash
git clone https://github.com/Girish2513/Smart-Nutri.git
cd Smart-Nutri
```

### 2. **Backend Setup (Django + DRF)**
```bash
cd backend
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```

🔹 Create a .env file inside the backend folder:
```env
SECRET_KEY=your_secret_key
DEBUG=True
DATABASE_URL=your_postgres_connection_string
```

🔹 Run Migrations and Start the Server:
```bash
python manage.py makemigrations
python manage.py migrate
python manage.py runserver
```

### 3. **Frontend Setup (React + Vite)**
```bash
cd ../frontend
npm install
```

🔹 Create a .env file inside the frontend folder:
```env
VITE_API_BASE_URL=http://127.0.0.1:8000
```

🔹 Start the Development Server:
```bash
npm run dev
```

## ▶️ Usage

- Open your browser and go to: http://localhost:5173
- Register or login using your credentials
- Add, edit, or delete appointments from the dashboard
- Filter and view appointments by status or date
- View upcoming appointments and appointment summary

## 🤝 Contributing

Contributions are welcome!

- Fork this repository
- Create a new feature or fix branch
- Make your changes
- Submit a pull request 🚀

## 📄 License

This project is licensed under the MIT License.
You are free to use, modify, and distribute this software.



## 💬 Contact

Developed with ❤️ by Girish Saana
- GitHub: @Girish2513
- Email: girishsaana2513@gmail.com
