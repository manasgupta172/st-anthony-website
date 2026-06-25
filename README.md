This is perfect. Having your actual GitHub username makes the open-source instructions fully complete.

Here is your finalized README.md with your exact repository links automatically wired in. You can copy this entire block and paste it directly into your GitHub repository to make it look incredibly professional for anyone visiting your profile!

Markdown
# St. Anthony's AI Chatbot 🏫🤖

[![Open Source Love](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://github.com/ellerbrock/open-source-badges/)
[![Next.js](https://img.shields.io/badge/Next.js-black?logo=next.js&logoColor=white)](https://nextjs.org/)
[![Flask](https://img.shields.io/badge/Flask-black?logo=flask&logoColor=white)](https://flask.palletsprojects.com/)
[![Gemini API](https://img.shields.io/badge/Google_Gemini-4285F4?logo=google&logoColor=white)](https://aistudio.google.com/)

A fully decoupled, full-stack Artificial Intelligence web application designed to serve as an instant digital assistant for St. Anthony's Sr. Sec. School. The chatbot provides immediate, context-aware answers regarding school admissions, faculty, student council, rules, and history.

## ✨ Features
* **Custom AI Brain:** Powered by the Google Gemini 3.5 Flash API, tightly constrained to school-specific knowledge using custom system instructions.
* **Decoupled Architecture:** A lightweight Python Flask backend API communicates with a modern Next.js React frontend.
* **Responsive UI/UX:** A custom-designed, fluid chat interface featuring typing animations, message history formatting, and mobile responsiveness.
* **Secure Environment:** API keys and sensitive endpoints are hidden server-side.

## 🛠️ Tech Stack

**Frontend (The Face)**
* Framework: Next.js (React)
* Styling: Tailwind CSS / Custom CSS
* Hosting: Vercel

**Backend (The Brain)**
* Framework: Python & Flask
* CORS Management: Flask-CORS
* AI Engine: Google Generative AI (Gemini)
* Hosting: Render (via Gunicorn)

---

## 🚀 Local Development Setup

If you want to run this project locally on your own machine, follow the steps below. Because this is a decoupled app, you will need to run two separate terminals.

### 1. Backend Setup (Flask API)
1. Clone the repository and navigate to the backend folder:
   ```bash
   git clone [https://github.com/manasgupta172/school-chatbot-backend.git](https://github.com/manasgupta172/school-chatbot-backend.git)
   cd school-chatbot-backend
Create a virtual environment and install the dependencies:

Bash
pip install -r requirements.txt
Create a .env file in the root of the backend folder and add your Gemini API Key:

Code snippet
GEMINI_API_KEY=your_google_api_key_here
Start the Flask server:

Bash
python server.py
The backend will now be running on http://localhost:5000

2. Frontend Setup (Next.js)
Open a new terminal window, clone the frontend repository, and navigate to the folder:

Bash
git clone [https://github.com/manasgupta172/school-chatbot-frontend.git](https://github.com/manasgupta172/school-chatbot-frontend.git)
cd school-chatbot-frontend
Install the Node modules:

Bash
npm install
Create a .env.local file in the root of the frontend folder and point it to your local backend:

Code snippet
NEXT_PUBLIC_API_URL=http://localhost:5000
Start the Next.js development server:

Bash
npm run dev
The website will now be running on http://localhost:3000

☁️ Deployment
This project is built to be deployed globally for free using Vercel and Render.

Backend: Connect your backend GitHub repository to Render as a Web Service. Set the Build Command to pip install -r requirements.txt and the Start Command to gunicorn server:app. Add your GEMINI_API_KEY to Render's environment variables.

Frontend: Connect your frontend GitHub repository to Vercel. Add NEXT_PUBLIC_API_URL to your Vercel environment variables, pointing it to your live Render URL.

🤝 Contributing
Contributions, issues, and feature requests are welcome! If you want to improve the UI, optimize the prompt engineering, or add new features, feel free to fork this repository and submit a Pull Request.

Fork the Project

Create your Feature Branch (git checkout -b feature/AmazingFeature)

Commit your Changes (git commit -m 'Add some AmazingFeature')

Push to the Branch (git push origin feature/AmazingFeature)

Open a Pull Request

👨‍💻 Author
Developed independently by Manas Class 12 PCM Student | Passionate about Computer Science & Applied AI If you found this project helpful, please consider giving it a ⭐ on GitHub!
