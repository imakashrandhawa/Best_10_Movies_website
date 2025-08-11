# 🎬 Best 10 Movies Website

A Flask-based web application where you can search, add, rate, and review your favorite movies.  
The site fetches movie details from **The Movie Database (TMDB) API** and stores them in a local database.


---

## 🚀 Features
- **Top 10 Movies** list ranked by rating
- **Add Movies** by searching TMDB
- **Edit Ratings & Reviews** via a simple form
- **Delete Movies** from the collection
- SQLite database for persistent storage
- Responsive design powered by **Bootstrap 5**

---

## 🛠️ Tech Stack
- **Backend:** Python, Flask, SQLAlchemy
- **Frontend:** HTML, Jinja2, Bootstrap 5
- **Database:** SQLite
- **API:** [TMDB API](https://developer.themoviedb.org/docs)

---

## 📦 Installation

1. **Clone this repository**
   ```bash
   git clone https://github.com/imakashrandhawa/Best_10_Movies_website.git
   cd Best_10_Movies_website
   ```

2. **Create and activate a virtual environment**
   ```bash
   python -m venv venv
   source venv/bin/activate   # Mac/Linux
   venv\Scripts\activate      # Windows
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

4. **Set up environment variables**
   - Create a `.env` file in the root directory:
     ```env
     key=Bearer YOUR_TMDB_READ_ACCESS_TOKEN
     SECRET_KEY=your_flask_secret_key
     ```
     *Note: `key` must include the word "Bearer " followed by your TMDB token.*

5. **Run the app locally**
   ```bash
   python main.py
   ```
   The app will be available at: `http://127.0.0.1:5000/`

---

## 🌐 Deployment
This app is deployed on [Render](https://render.com).  
To deploy:
- Push your code to GitHub
- Create a **Web Service** on Render
- Set the start command:
  ```bash
  gunicorn main:app
  ```
- Add environment variables (`key`, `SECRET_KEY`)
- Deploy and enjoy!

---


---

## 📜 License
This project is licensed under the MIT License. You are free to use, modify, and distribute it.

---

## 🙌 Acknowledgements
- [Flask](https://flask.palletsprojects.com/)
- [Bootstrap 5](https://getbootstrap.com/)
- [SQLAlchemy](https://www.sqlalchemy.org/)
- [TMDB API](https://developer.themoviedb.org/)
