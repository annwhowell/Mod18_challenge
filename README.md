# Mod18_challenge: Blockchain-based Ledger for Financial Transactions with Web Interface

#Overview
'''
This application creates a bloack-chain based ledger to facilitate the transfer of money (amount)
from one person (sender) to another (receiver). Each transaction is a new block in the chain.
The transfers are initited through a simpleweb-based interface created with Streamlit
'''

#Data and libraries
'''
Data is entered into the blocks via the web-based interface created by Streamlit

The program requires the following imports:

import streamlit as st
from dataclasses import dataclass
from typing import Any, List
import datetime as datetime
import pandas as pd
import hashlib
'''

#Coding
'''
The program uses a dataclass called Record

@dataclass
class Record:
    sender: str
    receiver: str
    amount: float


It uses the sha256 and encodes the data to create the hash

The pychain uses proof_of_work

Streamlit is used to create the Web-based interface to collect the sender, receiver and amount data

The code includes a Block Inspector function and 
Block difficulty can be set to 1, 5, 2

'''
# Run the code
#to run the code enter 'run streamlit pychain.py' in your terminal at the location of the file
#Your terminal will display locally hosted urls and should open the browser to the input webpage
#Example of url (and results of input/ hashes show in this image)
![<Terminal Display for Streamlit Launch>](<streamlit_terminal_results.png>)

# Results

#The data is entered on the webpage and the blocks and hashes are displayed

![<Data Entry and Resulting Blockchain with Hashes>](<pychain_screenshot1.png>)

#The blockchain inspector appears on the side and can help evaluate a specific block through the drop down

![<Block Inspector>](<block_inspector_screenshot.png>)

# License
MIT

# Created By
Ann Howell with support from Rice University FinTech Bootcamp
April 2022

