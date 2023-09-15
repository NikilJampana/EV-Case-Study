# EV-Case-Study
Teslas have been popping up everywhere around me, so I decided to take a deeper dive into understanding their recent surge in popularity in the form of a case study. 

# 1. Objective
EV owners and prospective owners have had growing concerns about EV charging according to a recent J.D. Power report. A company is trying to decide what locations are best to place EV charging stations in Washington. The task is to use existing data on EV populations and charging station availabity to identify areas to prioritize for placement of charging stations. The main data sets being used are an Electric Vehicle Population Dataset for the state of Washington and Federal records on Alternative Fueling Stations.

# 2. Data Cleaning and Preparation Steps
While there was little work to be done on the Electric Vehicle Population Dataset for the state of Washington, I did have to clean the Alternative Fueling Stations document. While it was originaly designed to represent several different types of alternative fuel across the United States, I filtered and adjusted the document to only look for electric charging station in Washington. In addition, the date format provided on the document wasn't compatible with Google Sheets, so I ran the csv through SQL to transfer it to a useable format for me. My data all originated from public data repositories from the U.S. Government, which verified its credibility for me and ensured that no licensing would prevent its personal use.




