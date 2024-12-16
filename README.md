# Dealspotr Coupon Scraper

This project is a web scraping tool built using Python and Selenium to scrape coupon codes and related data from various categories on the Dealspotr website.

---

## Project Overview

The scraper navigates through specific category pages on Dealspotr, clicks the **"View More"** button to load additional results, and extracts the following details from each product block:
1. **URL**: The promotional URL for the deal.
2. **Coupon Code**: The associated coupon code, if available.

The data is saved in an Excel file (`dealspotr_coupons.xlsx`) for further use.

---

## Features

1. **Automated Navigation**:
   - Automatically handles "View More" clicks to load more deals.
   
2. **Data Extraction**:
   - Extracts URLs and coupon codes from each deal entry.

3. **Data Storage**:
   - Saves the scraped data in a structured Excel format for analysis.

4. **Error Handling**:
   - Handles missing coupon codes and logs errors gracefully.

---

## Project Structure


---

## Prerequisites

1. **Install Python**:
   - Ensure Python 3.x is installed on your system.
   
2. **Install Dependencies**:
   - Use `pip` to install the required Python libraries:
     ```bash
     pip install selenium pandas openpyxl
     ```

3. **Download ChromeDriver**:
   - Download ChromeDriver from [here](https://sites.google.com/chromium.org/driver/) and place it in a suitable directory.
   - Update the `service` variable in the script to point to your ChromeDriver executable.

---

## How to Run

1. **Clone the Repository**:
   - Clone this repository to your local machine:
     ```bash
     git clone https://github.com/nishantshah2112/dealspotr-scraper.git
     ```
   
2. **Set Up the Script**:
   - Modify the `service` path in the script (`scraper.py`) to match the location of your ChromeDriver.

3. **Run the Script**:
   - Execute the scraper:
     ```bash
     python scraper.py
     ```

4. **Output**:
   - The extracted data will be saved in `dealspotr_coupons.xlsx`.

---

## Sample Data

| URL                                   | Coupon Code |
|---------------------------------------|-------------|
| https://dealspotr.com/example1        | SAVE10      |
| https://dealspotr.com/example2        | N/A         |
| https://dealspotr.com/example3        | FREEDEL     |

---

## Error Handling

- If the "View More" button is not found or an error occurs, the script will stop loading additional content and move on to extracting existing data.
- Missing coupon codes are logged as "N/A."

---

## Improvements

Here are some potential ways to enhance the project:
1. **Add More Categories**:
   - Extend the list of categories to scrape additional pages from Dealspotr.
2. **Dynamic Browser Handling**:
   - Add options for using different web browsers (e.g., Firefox or Edge).
3. **Data Analysis**:
   - Include a data analysis step to summarize coupon trends across categories.
4. **Real-Time Dashboard**:
   - Build a dashboard to display scraped data dynamically.

---

## Technologies Used

- **Python**:
  - Core language for scripting and data handling.
- **Selenium**:
  - For automating browser interactions.
- **Pandas**:
  - For structuring and saving data.
- **OpenPyXL**:
  - For exporting data to Excel.

---

## License

This project is licensed under the MIT License. See the LICENSE file for details.

---

## Contact

Feel free to reach out for any issues or suggestions:
- **Author**: Nishant Shah
- **GitHub**: [nishantshah2112](https://github.com/nishantshah2112)
