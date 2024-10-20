--
title	weight
Octoffers
1
--

## Overview

The `Djinni` class automates the job application process on the Djinni job platform (`djinni.co`) by scraping job listings, filtering them based on user-defined criteria, and submitting applications through Selenium WebDriver. This class is part of the Octoffers project and extends the functionality provided by the `Driver` class.

## Imports

- `os`, `sys`: Standard libraries for operating system and system-specific parameters.
- `dotenv`: For loading environment variables from a `.env` file.
- `re`: For regex operations.
- `selenium`: For web interaction, including:
  - `WebDriverWait`: To wait for elements to appear on the webpage.
  - Exceptions for error handling (`NoSuchElementException`, `TimeoutException`).
  - Various classes for locating elements (e.g., `By`, `EC`).
- `Driver`: Base class for managing the WebDriver.
- `db`: Database module for job data management.
- `get_cover_letter_from_openai`: Function to generate cover letters using OpenAI's API.

## Class Attributes

- **`JOB_FILTER`**: A query string used for filtering jobs based on keywords.

## Initialization

### `__init__(self, domain="djinni.co")`
- Initializes the Djinni class with the base URL and Chrome options for headless browsing.
- Sets the domain to `djinni.co` by default.

## Core Methods

### `_get_job_list(self, url)`
- Navigates to the specified URL and retrieves job listings using an XPath selector.
- Waits until the job items are present on the page.

### `_parse_salary(self, salary_text)`
- Extracts numeric values from a salary string using regex.
- Returns the minimum salary found or 0 if none is available.

### `fetch(...)`
- Retrieves job listings based on role, tools, minimum salary, exclusion words, and pages.
- Filters job postings and inserts valid entries into the database if they do not already exist.

### `apply(self, msg: str, ai_generated_letter: bool = False)`
- Automates the application process for jobs stored in the database that match criteria.
- Retrieves job entries, navigates to the job link, and submits a cover letter (user-provided or AI-generated).
- Updates the database to reflect the status of applications.

## Key Features

- **Headless Browsing**: Allows the automation to run without a visible browser window.
- **Dynamic Web Scraping**: Interacts with web elements to fetch job details and apply to listings.
- **Database Management**: Tracks job postings and application statuses using SQLite.
- **Error Handling**: Manages various exceptions to ensure smooth execution.
- **AI Integration**: Generates personalized cover letters using OpenAI's API.

## Conclusion

The `Djinni` class provides a robust solution for automating job applications on the Djinni platform. By integrating web scraping, database interactions, and AI capabilities, it streamlines the job search and application process effectively.
