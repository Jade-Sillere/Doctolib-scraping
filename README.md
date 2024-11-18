🏥 Doctolib Web Scraping Project
This project aims to build a comprehensive database on appointment availability of psychologists on Doctolib offering first-time consultations using the Selenium python package to scrape data from the popular French doctor bookings website Doctolib. The data collection is divided into two key steps, outlined below:

⚙️ Code Step 1: Collecting Basic Doctor Information
Objective
This step focuses on collecting essential details about psychologists listed on Doctolib who offer first-time consultations.

Description
The web scraping script retrieves basic doctor information, excluding specific appointment availability data. This data forms the core of the initial database and is used for subsequent processing and analysis.

Key Points:

The scraping process excludes fetching next available first-time psychology appointments (handled separately in Part II).
The resulting database includes foundational data (e.g., names, locations, specialties).

Script:

Jupyter Notebook - Selenium doctolib Part I



⚙️ Code Step 2: Completing the Database with Missing Information
Objective
This step focuses on enhancing the database with additional data that requires navigating to each psychologist's individual page.

Description
Given a dataframe containing the list of doctor names from Step 1, this code extracts the next available first-time psychology appointment date and time, if it is available.

Key Points:
Visits each doctor's profile page to gather detailed scheduling data.
This step complements the initial database by including appointment availability information.

Script:

Jupyter Notebook - Selenium doctolib Part II
