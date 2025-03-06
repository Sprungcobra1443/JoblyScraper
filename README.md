This Python-based tool is crafted to extract IT job listings from Jobly and organize them into an Excel file, facilitating easy access and analysis. The script meticulously captures essential details such as job title, company name, location, posting date, and company logo, providing a holistic view of each listing.

**Features**

- **Data Extraction:** Fetches IT job listings directly from Jobly.fi, ensuring up-to-date information.
- **Detail-Oriented:** Extracts specific elements including Job Title, Company Name, Location, Posting Date, and Company Logo URL, each stored meticulously.
- **Excel Output:** Seamlessly saves extracted data into an Excel file, enhancing accessibility for further analysis.
- **Console Display:** Provides immediate feedback by displaying job details in the console, offering quick reference for users.

**Technical Requirements**

To ensure smooth operation, the following Python libraries are essential:
- `selenium`
- `beautifulsoup4`
- `pandas`
- `openpyxl`
- `requests`
- `webdriver-manager`

**Installation Guide**

Install all necessary libraries with the following command:
```sh
pip install selenium beautifulsoup4 pandas openpyxl requests webdriver-manager
```

**Usage Instructions**

1. **Download the Script:** Obtain the `jobly_scraper.py` file via cloning or download to your local machine.
2. **Execution:** Run the script using Python:
   ```sh
   python jobly_scraper.py
   ```
3. **Expected Outcomes:** Upon successful execution, the script will display job details in the terminal and generate an Excel file named `IT_job_listings.xlsx` in the current directory.

**Operational Workflow**

1. **Request Initiation:** The script initiates a request to the Jobly IT jobs page.
2. **HTML Parsing:** Utilizes BeautifulSoup to parse the HTML content, ensuring efficient data extraction.
3. **Data Extraction:** Gathers job details, including Job Title, Company Name, Location, Posting Date, and Company Logo URL.
4. **Data Storage:** Organizes the extracted data into an Excel file for future reference and analysis.

**Output Details**

- **Console Output Example:**
  ```
  Job Title: Software Developer  
  Company: Google  
  Location: Helsinki  
  Date Posted: 25.01.2025  
  Company Logo: https://www.jobly.fi/logo_google.png  

  Job Title: IT Support Specialist  
  Company: Microsoft  
  Location: Tampere  
  Date Posted: 24.01.2025  
  Company Logo: https://www.jobly.fi/logo_microsoft.png  

  Data saved to IT_job_listings.xlsx
  ```
- **Excel File Structure:** The Excel file, `IT_job_listings.xlsx`, includes columns for Job Title, Company Name, Location, Date Posted, and Company Logo URL.

**Error Management**

- **Connection Issues:** In case of failure to access Jobly, an error message is displayed.
- **Data Handling:** Gracefully manages missing data with `None` values and leaves logo fields blank if absent.

**Limitations and Considerations**

- **Pagination:** Currently extracts data from the first page only.
- **HTML Dependency:** Performance may be affected by changes in Jobly's website structure.
- **Compliance:** Adherence to Jobly's terms of service is the user's responsibility.

**Conclusion**

Feel free to adapt and enhance this script to suit your needs. It serves as a robust foundation for IT job market analysis, offering both convenience and flexibility.