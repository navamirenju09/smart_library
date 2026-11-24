
# 📚 Smart Library

### AI-Powered Book Search & Recommendation System

Smart Library is an interactive Python web application developed during the **DevStorm Hackathon**.

The application helps users search for books, check their availability, and receive AI-powered recommendations when their desired books are unavailable.

---

## 🚀 Features

- **Personalized Welcome** — Greets users by name.
- **Library Categories** — Choose between Academic Textbooks and Leisure Reading.
- **Book Search** — Search for books by title.
- **Availability Tracking** — Check book availability and remaining copies.
- **AI Recommendations** — Suggests similar books using the Groq API.
- **Interactive Interface** — Built using Streamlit.

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| Python | Core application logic |
| Streamlit | Interactive web interface |
| Pandas | Dataset handling and filtering |
| Groq API | AI-powered book recommendations |
| CSV | Book database |
| python-dotenv | Environment variable management |

---

## ⚙️ How It Works

1. The user enters their name.
2. The user selects a library category.
3. The user searches for a book.
4. The application checks the CSV dataset.
5. If the book is available, the number of copies is displayed.
6. If the book is unavailable or not found, the application requests AI-generated recommendations.

---

## 📁 Project Structure

```text
smart_library/
│
├── book.py
├── book.csv
├── requirements.txt
├── .gitignore
└── README.md
```

---

## 💻 Installation & Setup

### 1. Clone the repository

```bash
git clone https://github.com/navamirenju09/smart_library.git
cd smart_library
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Configure the API key

Create a `.env` file in the project directory:

```env
GROQ_API_KEY=your_groq_api_key_here
```

Never upload your actual API key to GitHub.

### 4. Run the application

```bash
streamlit run book.py
```

The application will open in your browser.

---

## 📊 Dataset

The application uses `book.csv` to store library information.

The Python application expects columns named:

- `title`
- `category`
- `quantity`

The category values used for filtering are `academic` and `leisure`.

---

## 🤖 AI Integration

Smart Library integrates the Groq API to generate relevant book recommendations.

The application uses the `openai/gpt-oss-20b` model and asks it to recommend 1–3 books from a supplied list of library titles.

---

## 🏆 Hackathon

**Event:** DevStorm Hackathon

**Project:** Smart Library

**Type:** Team Project

Developed as a working prototype to explore Python application development, dataset management, and AI integration.

---

## 🔮 Future Improvements

- Filter recommendations to include only in-stock books.
- Improve book search and matching.
- Add book borrowing and return functionality.
- Introduce user authentication.
- Expand the library database.
- Improve recommendation accuracy.

---

## 👩‍💻 Developer

**Navami Renju**

B.Tech Computer Science Engineering

Lovely Professional University

[GitHub Profile](https://github.com/navamirenju09)

---

⭐ Built as part of my learning journey in software development.
