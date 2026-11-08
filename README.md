
# Structured LLM Prompt Pipeline & JSON Extractor

## Project Overview
This Python project uses Google Gemini AI to extract
structured information from unstructured resume text.

## Technologies
- Python 3
- Google Gemini API
- Pydantic
- python-dotenv
- JSON

## Features
- Reads resume text files
- Uses parameterized AI prompts
- Includes a few-shot example
- Extracts structured resume information
- Validates results using Pydantic
- Handles temporary Gemini server errors
- Saves validated results as JSON

## How to Run
1. Install Python 3.
2. Install dependencies from requirements.txt.
3. Create a .env file containing GEMINI_API_KEY.
4. Add resume information to resume.txt.
5. Run: python main.py

## Output
The program creates extracted_resume.json containing:
- Name
- Email
- Phone
- Education
- Skills
- Work experience

## Security
API keys are stored in .env and excluded from Git.

## Limitations
AI extraction can contain errors.
Pydantic validates data structure but cannot guarantee
that every extracted fact is correct.

## Testing Results

### Test 1: Complete Resume
Input: Maria Lopez, Occupational Therapist

Result:
- Successfully extracted resume information
- Generated validated JSON
- Saved output to extracted_resume.json

Status: PASSED

### Test 2: Missing Information
Input: James Wilson, Data Analyst

Result:
- Extracted name, email, education, and skills
- Correctly returned an empty phone field
- Generated validated JSON

Status: PASSED

### Test 3: Alternative Resume Format
Input: Sarah Johnson, Project Coordinator

Result: Pending

Status: NOT YET TESTED

## Key Learning Outcomes
- Python API integration
- Prompt engineering
- Structured JSON generation
- Pydantic data validation
- API error handling and retries
- Environment variable management
