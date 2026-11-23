# AI Resume Parser & Candidate Ranking System

An AI-powered Resume Screening and Ranking System that analyzes multiple resumes, extracts candidate information, matches skills with job requirements, and ranks candidates based on their suitability for a job role.

## 🚀 Features

- **Resume Parsing:** Extracts text and information from PDF resumes.
- **AI-Based Analysis:** Analyzes candidate profiles against job requirements.
- **Skill Matching:** Identifies matching and missing skills.
- **Candidate Scoring:** Calculates an overall job match percentage.
- **Candidate Ranking:** Ranks candidates based on their scores.
- **Experience Evaluation:** Checks whether candidates meet experience requirements.
- **Top & Lowest Candidates:** Displays the highest- and lowest-scoring candidates.

## 🛠️ Tech Stack

- Python
- Groq API
- Qdrant
- PyPDF
- python-docx
- uv (Python package manager)

## 📂 Project Structure

```text
AI-Resume-Parser/
│
├── src/
│   ├── day5/
│   │   └── __init__.py
│   │
│   ├── resumes/
│   │
│   └── resume_parser.py
│
├── resume_parser.py
├── .env
├── .gitignore
├── README.md
├── pyproject.toml
└── uv.lock
```

## ⚙️ Installation & Setup

### 1. Clone the repository

```bash
git clone https://github.com/ShivaYadav562/AI-Resume-Parser.git
```

### 2. Navigate to the project

```bash
cd AI-Resume-Parser
```

### 3. Create a virtual environment

```bash
uv venv --python 3.11
```

### 4. Activate the environment (Windows)

```powershell
.venv\Scripts\activate
```

### 5. Install dependencies

```bash
uv sync
```

### 6. Configure environment variables

Create a `.env` file in the project root:

```env
GROQ_API_KEY=your_groq_api_key
QDRANT_URL=your_qdrant_url
QDRANT_API_KEY=your_qdrant_api_key
```

Never upload your `.env` file or expose API keys publicly.

### 7. Add resumes

Place PDF resumes inside:

```text
src/resumes/
```

### 8. Run the project

```bash
python src/resume_parser.py
```

## 📊 Sample Output

```text
Processing: Abhay Resume.pdf
Score: 78.0

Processing: Ashish Resume.pdf
Score: 75.0

Processing: Shiva Resume.pdf
Score: 72.0

TOP 2 CANDIDATES

Abhay Pratap Singh - 78.0%
Ashish Raj - 75.0%

LOWEST 2 CANDIDATES

Ashish Raj - 75.0%
SHIVA YADAV - 72.0%
```

*Scores above are sample results from a development run.*

## 🎯 Project Objective

The objective of this project is to simplify the initial recruitment screening process by using AI to analyze resumes, identify relevant skills, evaluate candidates, and generate a ranked shortlist.

## 🔮 Future Improvements

- Web-based dashboard for recruiters.
- Support for DOCX resumes.
- Advanced candidate filtering.
- Resume upload interface.
- Downloadable candidate reports.
- Improved ranking and evaluation methods.

## 👨‍💻 Author

**Shiva Yadav**

- GitHub: [ShivaYadav562](https://github.com/ShivaYadav562)
- Project: [AI Resume Parser](https://github.com/ShivaYadav562/AI-Resume-Parser)

---

⭐ If you find this project useful, consider giving it a star!