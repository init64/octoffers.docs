---
title: "Djinni"
weight: 1
---

## Overview

The `Djinni` class automates the job application process on the Djinni platform (`djinni.co`) using Selenium WebDriver.

### Imports

- os, sys: Basic libraries for OS operations.
- dotenv: Loads environment variables.
- re: Regex operations.
- selenium: For web interaction and element handling.
- Driver: Base class for WebDriver management.
- db: Database module for job data.
- get_cover_letter_from_openai: Generates cover letters using OpenAI's API.

### Class Attributes

- JOB_FILTER: Query string for filtering jobs.

### Initialization

 `__init__(self, domain="djinni.co")`
- Initializes with the base URL and headless Chrome options.

### Core Methods

 `_get_job_list(self, url)`
- Retrieves job listings from the specified URL using XPath.

 `_parse_salary(self, salary_text)`
- Extracts numeric values from a salary string using regex.

 `fetch(...)`
- Retrieves job listings based on role, tools, salary, exclusion words, and pages.
- Filters job postings and inserts valid entries into the database.

 `apply(self, msg: str, ai_generated_letter: bool = False)`
- Automates job applications for stored entries.
- Submits a cover letter and updates the database.

### Key Features

- Headless browsing for automation.
- Dynamic web scraping for job details.
- Database management for tracking applications.
- Error handling for smooth execution.
- AI integration for personalized cover letters.

### Conclusion

The `Djinni` class eases the job search and application process on the Djinni platform through automation and AI capabilities.
