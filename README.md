
# Fintech Finder Application

This Python application uses Streamlit and Web3.py to interact with the Ethereum blockchain. The goal of the application is to enable users to hire fintech professionals using Ethereum cryptocurrency.

## Files

There are two main Python scripts in this application:

1. `fintech_finder.py`: This is the main script that provides the Streamlit user interface for the application. It allows users to interact with the Ethereum blockchain to send payments to fintech professionals.

2. `crypto_wallet.py`: This script contains several important functions for creating an Ethereum account, checking the balance of the account, and sending transactions to the Ethereum network.

## Functions

The `crypto_wallet.py` file provides the following functions:

1. `generate_account()`: This function creates a new Ethereum account using a mnemonic seed phrase.

2. `get_balance(w3, address)`: This function fetches the balance of Ether in a given Ethereum account.

3. `send_transaction(w3, account, to, wage)`: This function sends an authorized transaction to the Ethereum blockchain.

The `fintech_finder.py` file uses these functions to perform the following actions:

1. Generate a new Ethereum account instance.

2. Fetch and display the Ethereum account balance.

3. Calculate the total value of an Ethereum transaction, which includes the gas estimate and is used to pay a Fintech Finder candidate for their work.

4. Sign and send a transaction to the Ganache blockchain.

5. Review the transaction hash code.

6. Display Fintech Finder candidates, including their name, Ethereum address, rating, and hourly cost per Ether.

## Setup

To run this application, you will need to install the following Python libraries if they are not already installed:

- Streamlit
- Web3.py

Install these packages using pip:

```shell
pip install streamlit web3
```

You will also need to have a local Ethereum blockchain running, such as Ganache.

## Usage

Run the `fintech_finder.py` script in your terminal with Streamlit:

```shell
streamlit run fintech_finder.py
```

This will open the application in your web browser.
