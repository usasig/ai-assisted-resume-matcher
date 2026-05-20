# ai-assisted-resume-matcher

Job Hunt Assistant: AI-Powered Resume Matcher and Interview Insights Tool

## Overview

This tool helps job seekers find relevant director and manager level positions, compare them against your resume, identify gaps, and research what actually worked for successful candidates in those roles.

## Core Features

1. **Job Discovery** - Searches multiple job boards for director and manager openings in your target industry or location.
2. **Resume Analysis** - Parses your uploaded resume to extract skills, experience, certifications, and education.
3. **Gap Analysis** - Compares job requirements against your resume and flags missing or weak criteria that are crucial for the role.
4. **Interview Intelligence** - Pulls hiring patterns and interview insights from LinkedIn, Indeed, Reddit, Levels.fyi, Blind, and company career pages to show what skills and experiences helped successful candidates.
5. **Actionable Feedback** - Provides a prioritized list of top job matches with a clear roadmap of what to strengthen on your resume before applying.

## Architecture

The system has four main modules:

- **Job Scraper** - Fetches postings from Indeed, LinkedIn, and company career pages using web APIs or web scraping libraries.
- **Resume Parser** - Extracts structured data from uploaded resume files (PDF or text).
- **Gap Analyzer** - Compares resume content against job requirements.
- **Interview Insights Engine** - Aggregates hiring patterns and interview data from multiple sources.

## Tech Stack Recommendations

**Backend:**
- Python with Flask or FastAPI for the API layer
- Libraries: BeautifulSoup or Selenium for web scraping, PyPDF2 or pdfplumber for resume parsing, requests for HTTP calls, spaCy or NLTK for NLP

**Frontend:**
- Simple web interface using React or Vue to upload resumes and display results
- Or build it as a Claude Project integration

**Data Sources:**
- Indeed API
- LinkedIn job search
- Reddit API
- Levels.fyi
- Blind
- Company career pages
- PayScale

## Workflow

1. **Step 1** - User uploads resume in PDF or text format
2. **Step 2** - System parses resume and extracts key information
3. **Step 3** - User inputs target job title, industry, or company
4. **Step 4** - System searches for matching positions
5. **Step 5** - Gap analysis and interview insights are generated
6. **Step 6** - User receives prioritized job matches with actionable feedback

## Getting Started

1. Set up a Python virtual environment
2. Install dependencies listed in `requirements.txt`
3. Configure API keys for Indeed, LinkedIn, Reddit, and other data sources
4. Build the resume parser module first

### Next Steps

- Start with the resume parser to understand your resume structure
- Then move to the job scraper for one source like Indeed
- Once those work, layer in gap analysis
- Leave interview insights for later phases as it requires more data sources
