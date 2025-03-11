# **Peace Project Web Scraping**  

## **Overview**  
This repository contains the web scraping component of the **Peace Project**, which aimed to analyze the relationship between a world leader’s background—specifically whether they lived abroad—and their propensity to engage in conflict. This component focused on **automating the extraction of biographical data** on world leaders from various online sources to support the larger research effort.  

## **Research Goals**  
- **Collect structured biographical data** on world leaders from reliable sources  
- **Extract key attributes** such as birth country, education, career history, and international experiences  
- **Standardize and clean** extracted data for use in NLP-based classification (see [Peace Project](https://github.com/cmoser11/peace_project))  
- **Store data efficiently** for further analysis  

## **Methodology**  
### **1. Web Scraping Process**  
- Used **BeautifulSoup** and **Requests** to scrape leader biographies from publicly available sources  
- Implemented **Selenium** for dynamic content extraction on JavaScript-heavy websites  
- Extracted key data points, including:  
  - Name  
  - Birthplace  
  - Education  
  - Career history  
  - Known time spent living abroad  

### **2. Data Cleaning & Processing**  
- Standardized **location names and dates**  
- Removed duplicate entries and missing values  
- Structured data into a **CSV format** for easy integration into downstream analysis  

### **3. Data Storage & Export**  
- Saved cleaned data in a structured CSV file:  
  ```plaintext
  | Name          | Birth Country | Education               | Career History | Lived Abroad (Y/N) |
  |--------------|--------------|-------------------------|---------------|------------------|
  | Leader A     | France       | University of Paris    | Diplomat      | Yes              |
  | Leader B     | USA          | Harvard University     | Senator       | No               |
  ```  

## **Technologies & Tools**  
- **Web Scraping:** BeautifulSoup, Selenium, Requests  
- **Data Processing:** Pandas, NumPy  
- **Storage Format:** CSV  


## **Next Steps**  
- Expand scraping sources to **increase dataset coverage**  
- Improve **data extraction accuracy** using NLP techniques  
- Integrate **named entity recognition (NER)** for better data structuring  
- Connect with the **Peace Project NLP pipeline** to analyze leaders' backgrounds  

