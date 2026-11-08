# Datheon Python + Generative AI & LangChain Internship

## Project Overview

This repository documents my hands-on projects completed as part of the Datheon Python + Generative AI & LangChain Internship program.

The purpose of this internship is to strengthen my practical experience in Python programming, large language models (LLMs), prompt engineering, API integration, structured data extraction, and AI application development.

Each project is organized into a separate folder with its source code, documentation, sample inputs, and outputs.

## Internship Projects

### Task 1: Structured LLM Prompt Pipeline & JSON Extractor

**Status: Completed and tested**

**Project Description:**

Developed a Python application that uses the Google Gemini API to extract structured information from unstructured resume documents.

The application converts resume text into a validated JSON format using Pydantic.

**Technologies Used:**
- Python 3
- Google Gemini API
- Pydantic
- JSON
- python-dotenv
- Git and GitHub

**Key Features:**
- Integration with a large language model through an API
- Parameterized prompt templates
- Few-shot prompting
- Structured JSON output generation
- Pydantic schema validation
- Missing-information handling
- Automatic retries for temporary API server errors
- Secure API key management using environment variables

**Testing:**

Tested the application with two fictional resumes representing different professional backgrounds.

- Test 1: Occupational Therapist resume — successfully extracted structured information.
- Test 2: Data Analyst resume — successfully extracted structured information and correctly handled a missing phone number.

**Outcome:**

Successfully developed and tested an executable Python script that converts unstructured resume information into validated JSON output.

**Project Folder:** `Task_1_JSON_Extractor/`

### Task 2: Upcoming Project

**Status: Not yet completed**

The official project description, implementation, and testing results will be added after completing Task 2.

## Repository Structure

```text
Datheon Internship/
│
├── README.md
├── .gitignore
│
└── Task_1_JSON_Extractor/
    ├── README.md
    ├── main.py
    ├── resume.txt
    ├── extracted_resume.json
    └── requirements.txt
```

Additional task folders will be included as projects are completed.

## Getting Started

1. Install Python 3.
2. Clone the repository.
3. Navigate to `Task_1_JSON_Extractor`.
4. Install dependencies using `pip install -r requirements.txt`.
5. Create a private `.env` file in the repository root.
6. Add `GEMINI_API_KEY=your_api_key_here` to `.env`.
7. Run `python main.py`.

## Security and Privacy

API credentials are stored locally in environment variables and excluded from Git version control using `.gitignore`.

All sample resume information used for testing is fictional.

## Skills Developed

- Python programming
- Generative AI integration
- LLM prompt engineering
- JSON data extraction
- Pydantic validation
- API troubleshooting and error handling
- Git version control
- Technical documentation

## Future Development

Future improvements may include PDF resume processing, batch document extraction, additional validation rules, and integration with LangChain.

## Internship Submission

This repository is being prepared for review under the Datheon Python + Generative AI & LangChain Internship program.

**Submission Status:** In progress — additional required task(s) pending completion.