---
title: "Djinni"
weight: 1
---

## Overview

The `Djinni` class automates job applications on Djinni (djinni.co) using Selenium WebDriver.

### Imports

- os, sys: For OS operations.
- dotenv: Loads environment variables.
- re: Regex operations.
- selenium: For web interaction.
- Driver: Manages WebDriver.
- db: Database for job data.
- get_cover_letter_from_openai: Generates cover letters via OpenAI.

### Class Attributes

- JOB_FILTER: Query string for filtering jobs.

### Initialization

- Sets base URL and headless Chrome options.

### Core Methods

- `_get_job_list(url)`: Retrieves job listings using XPath.
  
- `_parse_salary(salary_text)`: Extracts numeric salary values using regex.
  
- `fetch(...)`: Fetches and filters job listings, Adding valid entries into the database.
  
- `apply(msg, ai_generated_letter=False)`: Automates applications, submits cover letters, and updates the database.

### Key Features

- Headless browsing.
- Web scraping for job details.
- Database for tracking applications.
- AI-generated cover letters.

### Conclusion

The `Djinni` class simplifies job search and applications on Djinni through automation and AI.
