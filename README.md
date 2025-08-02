## JobScrape

This Python script **automatically collects job listings** from [Techversant Infotech's careers page](https://techversantinfotech.com/talent/) and **saves them into an Excel file**.



## 🤔 What It Does

- Visits Techversant's job listings page.
- Extracts details such as:
    - Job Title
    - Category
    - Location
    - Posting Date
    - Required Skills
    - Experience Needed
    - Contact Email
- Organizes all information into a styled Excel file named `Techversant_Jobs.xlsx`.



## 📦 Requirements

### ✅ Step 1: Create a virtual environment

```bash
python -m venv venv
```

### ✅ Step 2: Activate the virtual environment

- **Windows**:

    ```bash
    venv\Scripts\activate
    ```

- **Mac/Linux**:

    ```bash
    source venv/bin/activate
    ```

### ✅ Step 3: Install dependencies

```bash
pip install -r requirements.txt
```



## 🧠 How to Use

1. Ensure Python is installed on your system.
2. Open a terminal and navigate to the project folder.
3. Follow the steps in the Requirements section to set up the environment.
4. Run the scraper:

     ```bash
     python scrape.py
     ```

5. If successful, the Excel file `Techversant_Jobs.xlsx` will be created in the same folder.




## 📊 Output

The Excel file includes:

- A `Jobs` sheet with:
    - JobTitle
    - JobCategory
    - Location
    - ExperienceRequired
    - PostingDate
    - JobDescriptionSummary
    - SkillsRequired
    - ContactEmail
    - CompanyBenefits
    - Salary
    - JobURL
    - JobID
    - ScrapedDate
    - SourceURL

- A `Summary` sheet with:
    - Total job count
    - Breakdown by category and location
    - Date of scraping


## 💡 Notes

- Only scrapes the **first page** of job listings (pagination detection is implemented).
- If Techversant updates their website layout, the script may require adjustments.


## 👨‍💻 Author

Built with ❤️ by Arjun  
For automation, scraping, and data tasks.
