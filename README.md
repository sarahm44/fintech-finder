# FinTech Finder - Cryptocurrency Wallet

![](/Images/19-4-challenge-image.png)

## Overview 

Fintech Finder is an application that its customers can use to find fintech professionals from among a list of candidates, hire them, and pay them. 

I was tasked with integrating the Ethereum blockchain network into the application in order to enable customers to instantly pay the fintech professionals whom they hire with cryptocurrency.

I completed the code that enables customers to send cryptocurrency payments to fintech professionals. 

To develop the code and test it out, I assumed the perspective of a Fintech Finder customer who is using the application to find a fintech professional and pay them for their work.

## Relevant Files

### FinTech Finder

The [fintech_finder.py](fintech_finder.py) file contains the code associated with the web interface of the application. 

The code included in this file is compatible with the [Streamlit](https://streamlit.io/) library. 

### Crypto Wallet

The [crypto_wallet.py](crypto_wallet.py) file contains Ethereum transaction functions. 

By using import statements, I integrated the crypto_wallet.py Python script into the Fintech Finder interface program that is found in the [fintech_finder.py](fintech_finder.py) file.

### Integrating the Two Files

Integrating these two files automates the tasks associated with generating a digital wallet, accessing Ethereum account balances, and signing and sending transactions via a personal Ethereum blockchain called Ganache.

## Testing the Application

The steps for testing out the application are as follows:

* Import Ethereum Transaction Functions into the Fintech Finder Application
* Sign and Execute a Payment Transaction
* Inspect the Transaction on Ganache

Below is the resulting webpage from running the Streamlit app:

![Alt_text](/Screenshots/screenshot1.png)

To test the app, I chose a candidate I would like to hire. Then, I entered the number of hours that I would like to hire them for:

![Alt_text](/Screenshots/screenshot2.png)

I then navigated to the Transactions section of Ganache. See below a screenshot of my address balance and history on Ganache:

![Alt_text](/Screenshots/screenshot5.png)

Below is a screenshot of the transaction details on Ganache:

![Alt_text](/Screenshots/screenshot3.png)

I then returned to the original transaction, and clicked the transaction’s To address. Below is a screenshot of the recipient’s address balance and history from my Ganache application:

![Alt_text](/Screenshots/screenshot4.png)

