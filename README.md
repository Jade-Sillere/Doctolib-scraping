# 🏥 Doctolib Web Scraping Project
This project aims to build a comprehensive database on appointment availability of psychologists on Doctolib offering first-time consultations using the Selenium python package to scrape data from the popular French doctor bookings website Doctolib. The data collection is divided into two key steps, outlined below:

## ⚙️ Code Step 1: Collecting Basic Doctor Information
### Objective
This step focuses on collecting essential details about psychologists listed on Doctolib who offer first-time consultations.

### Description
The web scraping script retrieves basic doctor information, excluding specific appointment availability data. This data forms the core of the initial database and is used for subsequent processing and analysis.

### Key Points:
The scraping process excludes fetching next available first-time psychology appointments (handled separately in Part II).
The resulting database includes foundational data (e.g., names, locations, specialties).

### Script:
Jupyter Notebook - Selenium doctolib Part I



## ⚙️ Code Step 2: Completing the Database with Missing Information
### Objective
This step focuses on enhancing the database with additional data that requires navigating to each psychologist's individual page.

### Description
Given a dataframe containing the list of doctor names from Step 1, this code extracts the next available first-time psychology appointment date and time, if it is available.

### Key Points:
Visits each doctor's profile page to gather detailed scheduling data.
This step complements the initial database by including appointment availability information.

### Script:
Jupyter Notebook - Selenium doctolib Part II

## ⚠️ Considerations
Scraping the Doctolib website can be challenging due to potential timeouts caused by a high volume of requests and rotating search results. To mitigate these issues, the following measures were implemented:

Proxy Rotators: To prevent IP bans and distribute requests more evenly.
Random Timers: Introducing delays between requests to simulate human browsing behavior.
Simulated Human Interaction: Randomized scrolling and clicking patterns to mimic typical user activity.
Given time constraints, the best strategy is to:

Limit Timer Lengths: This helps optimize run-time while maintaining effectiveness.
Partial Saves: Save data incrementally to avoid data loss during long scraping sessions.
Remove Duplicates: Use the practice ID to eliminate duplicate entries.

## 📦 Required Packages
Ensure the following packages are installed before running the scripts:

Selenium
Pandas

If they are not installed, simply run the following command in your command prompt.
pip install selenium pandas
