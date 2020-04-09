## Proposal name:
arweave-news-bot

## Summary:
I would like to create a news archive using data provided by newsapi.org 

The data will be stored on the arweave network in json format.

This script will be written in a way that it can by be used by many different bot operators and many users per bot operator without excessively duplicating content.

## Motivation:
I want to do this to create a way for multiple bot operators to archive news api data on the arweave network. 

Arweave could gain by increased use of the network and increased usability. 

This data would be available to all developers using ARQL.

Anyone with a linux server and AR could participate in adding data to the news archive.

This data could possibly be used to automate archival of news articles to the Arweave network in the future.

## Specification:
I will fork the existing news permafeed script located at https://github.com/crypto-guys/arweaveNewsPermafeed

The existing MIT License will remain in place.

Planned Script Improvements 
    - Allow for all available search parameters from newsapi.org
    - Search parameters will be input using input form or the config.sh file depending on owners requirements
    - Ensure a data tag exists for each configured search parameter 
    - Search Parameters are (keyword, keywordintitle, sources, domains, excludeDomains, fromdate , todate, sortby, pagesize)
    - Ensure a data tag exists for each configured search parameter
    - Add functionality to get all pages of results, this will allow the bot to retrieve any amount of results
    - Reorganize to allow for easy updates and better functionality without code duplication
    - Create one time run option to allow for archival when the single run would return millions of results taking multiple days to retrieve
    - Add more logging features in case of interruption to resume from last position
    - Improve on current logging as needed
    - Ensure hourly, twice daily and daily schedules are working as designed. Possibly change frequency as required.
    - Add or remove scheduling options as required.
    - Add data validation with ARQL as source when starting the bot to avoid duplicate data archives where possible
    - Add validation to check for errors from the api
    - Create a simple front end interface to submit new keyword search requests and to allow users to specify search parameters.
    - Users submit a keyword search request and a new wallet will be generated then the user will be supplied the address to deposit into tags will be used for wallet management
    - Allow bot owner to specify owner wallet in config
    - Allow bot owner to specify the % of incoming funds to send to owner wallet for operational costs in config
    - Add functionality to automatically remove the specified % of incoming funds from the newly generated address and send to owner wallet
    - The bot will run until the funding wallet is empty. To continue running your keyword search simply deposit more funds before the wallet address is empty. 
    - Monitor wallets for new deposits all new deposits reset search parameters and keywords so they must include tags.
    - I will test by creating a keyword search for coronavirus and specify a start date of 30 days prior to testing date. Once that data is archived the bot should automatically change to a more compatible schedule.
    - My test will run until 6 AR have been used.
    
    
    This is likely not an all inclusive list of the changes that will be required. I plan to allow input from the ARCA group and work with them to provide something that works well. I am a flexible guy :) I just want to make something useful. If something is needed that is not in this list and time allows I would be happy to add it.

## Team and previous work:
This is my previous work.

https://github.com/crypto-guys/

https://github.com/pinkgoatcheese/

## Timeline:
I would ask that I be allowed up to 15 days to complete the upgrade. This will ensure quality code, allow time for testing,  and allow for any unforeseen problems that could occur. 


## Grant requested (DAI):
400 DAI Upfront
600 DAI Upon Completion.


## Ethereum Address:
0x3D6087EbC73fb4f6d961a42076fA43A0Ae4e425c
