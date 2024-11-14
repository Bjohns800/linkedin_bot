# LinkedIn Job Saver

A Python script that automates the process of saving LinkedIn job postings as PDFs for future reference. This tool is perfect for job seekers who want to efficiently track job postings and maintain a personal archive of job descriptions.

## Features
- **Automated job scraping**: Automatically saves LinkedIn job listings to PDFs.
- **Easy tracking**: Stores job information (e.g., job title, company, location) in a CSV file.
- **Customizable searches**: Easily modify search parameters to target specific roles and locations.

## Requirements
Before running the script, ensure you have the following installed:

- **Python 3.8** or higher
- **Selenium** (Install using: `pip install selenium`)
- **ChromeDriver** (compatible with your installed Chrome browser version)

### Optional
If a `requirements.txt` file is provided, you can install all dependencies with:
```bash
pip install -r requirements.txt
Installation
Clone the repository and install the necessary dependencies:

bash
Copy code
git clone https://github.com/your-username/linkedin-job-saver.git
cd linkedin-job-saver
pip install selenium
Download and Configure ChromeDriver
Download ChromeDriver (ensure it matches your Chrome browser version).
Place the chromedriver executable in your system's PATH or in the project directory.
Usage
1. Set Up LinkedIn Credentials
Open the script (linkedin_job_saver.py) and update the following variables with your LinkedIn credentials:

python
Copy code
USERNAME = "your_email@example.com"
PASSWORD = "your_password"
⚠️ Warning: Avoid sharing your credentials or uploading them to public repositories. Consider using environment variables for added security.

2. Customize Your Job Search
Modify the search parameters in the script to match your job preferences:

python
Copy code
search_keywords = "Python Developer"
location = "New York, NY"
3. Run the Script
To start the job scraping process, run:

bash
Copy code
python linkedin_job_saver.py
4. Review Saved Jobs
The job postings will be saved to a CSV file (e.g., jobs.csv) and PDFs in the saved_jobs folder for easy reference.

Example
Here's an example of modifying the search parameters:

python
Copy code
# Sample search parameters in the script:
search_keywords = "Data Analyst"
location = "San Francisco, CA"
Troubleshooting
ChromeDriver Issues: Ensure your ChromeDriver version matches your installed Chrome browser version. Check your Chrome version by navigating to chrome://version/.
Selenium Errors: If you encounter issues with Selenium, make sure all dependencies are up to date:
bash
Copy code
pip install --upgrade selenium
CAPTCHA Verification: LinkedIn may prompt for CAPTCHA verification during login. You may need to solve it manually or adjust the script to include longer delays between actions.
Notes
Ensure your LinkedIn account is in good standing to avoid potential restrictions due to automation.
Be mindful of LinkedIn's terms of service regarding automated scraping.
License
This project is licensed under the MIT License. See the LICENSE file for more details.
