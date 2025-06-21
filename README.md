# BTD6-Tower-Calculator
## This project aims to provide Bloons Tower Defense 6 (BTD6) players with a user-friendly application to determine the in-game cost of tower units and their upgrades across different difficulties.
The final project can be accessed using this [Google Sheets link](https://docs.google.com/spreadsheets/d/1bgRTX8VRlwiGp4RJNIbdQKh3tUHXspOqAZUE-NDchDM/edit?usp=sharing). 


--- 

## Define - Overview
This objective of this project was to develop a user friendly application for Bloons Tower Defense 6 (BTD6) players to be able to determine how much a in-game Tower unit cost. This project includes utilizing Python to acquire and organize data, Google Sheets to create calculation formulas, allow easy user accessibility and interaction with the app. 

### Features & Functionality
- Cost Calculation: Calculates the cost of BTD6 towers and their upgrades.
- Difficulty-Based Pricing: Accounts for different in-game difficulties (Easy, Medium, Hard, Impoppable).
- Interactive Interface: Google Sheets dropdown menus for user accessibility and interaction,

## Project Structure / How it was made
This project combines 2 major elements: 
- Python scripting for robust data acquisition and data cleaning 
- data cleaning with Google Sheets for an accessible and interactive user experience.

### Data Collection (BloonsProject.ipynb)
The BloonsProject.ipynb is a jupyter notebook used to prepare the projects data. This included: 

1) **How the Data is First Gathered (Automated Collection)**
The first step was to get tower cost information directly from the Bloons TD 6 Fandom Wiki. This project uses Python to webscrape the HTML data from the Wiki, and automatically acquire all the tower names, upgrade paths, and their costs without manual input. This data is unrefined from the initial webscraping, and needs improvements before its used.

2) **Data Cleaning and transformation:**
After collecting the raw information about tower costs from the Bloons Fandom Wiki, the data was messy and required several steps to make it useable:

The collected costs are initially presented in a way that might be hard to work with directly. Rows and columns had multiple data points in each row. 
-The raw data often includes extra words, symbols, or formatting alongside the actual cost numbers (e.g., "Cost: 100 Cash" or "Upgrade Price $50").

The project then rearranges and organizes this data. It clearly separates the costs based on:
- Game Difficulty: Distinguishing prices for Easy, Medium, Hard, and Impoppable modes.
- Upgrade Tiers: Categorizing costs for each specific upgrade level (Tier 1 through Tier 5) along different upgrade paths.

This structuring creates a consistent and easy-to-use dataset, and exports the data into a excel spreadsheet for further processing. 
