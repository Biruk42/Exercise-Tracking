# Exercise Tracker

This Python script allows users to track their exercises by sending a request to the Nutritionix API, recording the workout data in a Google Sheets document.

## Prerequisites

Before running the script, ensure you have the following:

- Python 3 installed on your machine.
- `requests` library installed. If not, you can install it using pip:

- An account with Nutritionix to obtain API credentials.
- An environment with Google Sheets API access, or other spreadsheet services that accept HTTP requests.

## Setup

1. Clone the repository or download the script.
2. Install the necessary Python packages.
3. Obtain API credentials from Nutritionix.
4. Set up a spreadsheet to record exercise data. If you're using Google Sheets, enable the Google Sheets API and obtain the sheet endpoint.
5. Set up environment variables for your API credentials and sheet endpoint.

## Usage

1. Run the script.
2. When prompted, enter the exercises you performed.
3. The script will make a request to the Nutritionix API to retrieve exercise details and record them in the specified spreadsheet.

## Environment Variables

Ensure you have the following environment variables set:

- `YOUR_APP_ID`: Your Nutritionix API App ID.
- `YOUR_API_KEY`: Your Nutritionix API Key.
- `YOUR_SHEET_ENDPOINT`: The endpoint of your spreadsheet service.
- Optionally, for Basic Auth or Bearer Token authentication:
- `USERNAME`: Your username for Basic Auth.
- `PASSWORD`: Your password for Basic Auth.
- `TOKEN`: Your bearer token for Bearer Token authentication.

## Script Explanation

- The script begins by importing necessary libraries and setting constants such as gender, weight, height, and age.
- It collects exercise input from the user and sends a request to the Nutritionix API to get exercise details.
- The obtained data is then formatted and recorded in the spreadsheet.
- The script supports three authentication methods for sending data to the spreadsheet: No Auth, Basic Auth, and Bearer Token. You can choose the appropriate method based on your spreadsheet service's authentication requirements.
