# Resume Information Extractor using Gemini API

An AI-powered Resume Information Extractor that extracts structured information from PDF resumes using Google's Gemini API.

The project converts unstructured resume content into clean, structured JSON data with the help of **Gemini AI, Pydantic validation, error handling, retry mechanisms and logging**.

## Features

- **PDF Upload:** Upload resumes in PDF format.
- **Text Extraction:** Extract text from PDF files using PyPDF.
- **Gemini API Integration:** Use Gemini 2.5 Flash to extract resume information.
- **Structured Data Extraction:** Extract name, email, phone number, skills, education and years of experience.
- **Pydantic Validation:** Validate and clean extracted information.
- **Improved Prompt Engineering:** Use clear instructions to reduce incorrect or fabricated information.
- **Retry Mechanism:** Automatically retry temporary API failures using exponential backoff.
- **Logging:** Track application events, successful operations and errors.
- **JSON Output:** Save validated resume information into a JSON file.
- **Error Handling:** Handle invalid PDFs, missing files, API errors and validation failures.

## Technologies Used

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Google Gemini API | AI-based information extraction |
| Gemini 2.5 Flash | Language model |
| Pydantic | Data validation |
| PyPDF | PDF text extraction |
| JSON | Structured data storage |
| Logging | Application monitoring |

## 📂 Extracted Information

The application extracts the following fields:

| Field | Description |
|---|---|
| name | Candidate's name |
| email | Email address |
| phone | Phone number |
| skills | List of technical and other skills |
| education | Educational qualifications |
| experience_years | Total years of experience |

## ⚙️ Installation and Setup

### 1. Clone the repository

```bash
git clone https://github.com/your-username/resume-information-extractor.git
```

### 2. Install required packages

```bash
pip install google-genai pydantic pypdf
```

### 3. Get a Gemini API Key

Get your API key from:

https://aistudio.google.com/apikey

### 4. Run the application

The current implementation uses Google Colab for PDF upload and downloading files.

Open the notebook in Google Colab, execute the cells and enter your Gemini API key when prompted.

## 🔄 Project Workflow

1. Upload a PDF resume.
2. Extract text using PyPDF.
3. Create an improved extraction prompt.
4. Send the prompt to Gemini 2.5 Flash.
5. Receive structured JSON data.
6. Validate the response using Pydantic.
7. Retry temporary API failures when necessary.
8. Log application activities and errors.
9. Display and save the final JSON output.

## 📁 Output Example

```json
{
    "name": "Rahul Sharma",
    "email": "rahul@example.com",
    "phone": "9876543210",
    "skills": [
        "Python",
        "Java",
        "SQL",
        "Machine Learning"
    ],
    "education": "B.Tech Computer Science",
    "experience_years": 2
}
```

*Example output for demonstration purposes.*

## 📋 Generated Files

- `resume_extracted.json` – Contains validated resume information.
- `resume_extractor.log` – Stores application logs.

## 🔐 Security

- API key is entered securely using `getpass`.
- API keys should never be hardcoded or uploaded to GitHub.
- Resume information is processed using the Gemini API.

## 🔮 Future Improvements

- OCR support for scanned PDF resumes.
- Duplicate skill removal.
- More advanced validation.
- Support for multiple resume formats.
- Automated resume ranking and skill matching.
- Unit testing for validation and error handling.

## 👩‍💻 Author

TEJASHWINI SRIGADDE

B.Tech Computer Science Engineering Student

---

⭐ If you find this project useful, consider giving it a star!
