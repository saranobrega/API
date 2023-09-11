# API-Explorations
A collection of notebooks and scripts showcasing various API interactions 

Content:

## BankAPI 

This Flask-based web API provides functionality for managing user accounts and transactions. It includes features such as user registration, adding money, transferring funds, checking balances, taking loans, and paying loan


### Getting Started
To run this API locally or deploy it to a server, follow these instructions:


### Prerequisites
- Python 3.x
- Flask
- Flask-RESTful
- pymongo
- bcrypt
```
pip install Flask Flask-RESTful pymongo bcrypt
```
### API Endpoints
- /register: POST endpoint to register a new user. Send a JSON object with the username and password to create an account.
- /add: POST endpoint to add money to a user's account. Provide the username, password, and the amount to be added.
- /transfer: POST endpoint to transfer money between users. Specify the sender's username, password, the recipient's username, and the amount.
- /balance: POST endpoint to check the account balance. Provide the username and password to get the balance.
- /takeloan: POST endpoint to take a loan. Send the username, password, and the loan amount.
- /payloan: POST endpoint to repay a loan. Provide the username, password, and the repayment amount.


### Running the API
```
uvicorn app:app
```
### Example Usage
- Register a New User
```
{
  "username": "newuser",
  "password": "password123"
}
```
- Add Money to Account
```
{
  "username": "user1",
  "password": "password123",
  "amount": 100
}
```
## Featured Notebooks:
**GitHub Repository Data Collection:**
This notebook demonstrates how to fetch repository data from a GitHub user profile. It covers:
- Making GET requests to the GitHub API.
- Extracting specific data points like repository name, description, and creation date.
- Formatting and processing the retrieved data.
- Storing the processed data in a pandas DataFrame for further analysis.

## Usage
To use the notebooks:

Clone the repository.
Install the required libraries (e.g., requests, pandas).
Open the desired notebook and run the cells.

## Contributions
Feel free to fork this repository and add your own API exploration notebooks. Pull requests with improvements, optimizations, or new techniques are always welcome.
