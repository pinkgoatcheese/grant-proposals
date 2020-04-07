## Proposal name:
arweave-news-bot

## Summary:
I would like to create a news archive using data provided by newsapi.org 

The data will be stored on the arweave network in json format.

This script will be written in a way that it can by be used by many different bot operators without excessively duplicating content.

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
    * Add config features to allow for all available search parameters from newsapi.org
        (keyword, keywordintitle, sources, domains, excludeDomains, fromdate , todate, sortby, pagesize)
    * Ensure a data tag exists for each configured search parameter
    * Add functionality to get all pages of results, this will allow the bot to retrieve any amount of results
    * Reorganize to allow for easy updates and better functionality
    * Create one time run option to allow for archival when the single run would return millions of results taking multiple days to retrieve
    * Add more logging features in case of interruption to resume from last position
    * Improve on current logging as needed
    * Ensure hourly, twice daily, and daily scheduling options work as intended 
    * Add data validation with ARQL as source when starting the bot to avoid duplicate data archives where possible
    * Add validation to check for errors from the api
    * Allow bot owner to specify owner wallet in config
    * Allow bot owner to specify the % of donations to send to owner wallet for operational costs in config
    * Add functionality to check bot wallet balance and automatically remove specified % of incoming funds then send to owner wallet

## Team and previous work:
This is my previous work.

https://github.com/crypto-guys/

https://github.com/pinkgoatcheese/

## Timeline:
I would ask that I be allowed up to 14 days to complete the upgrade. This will ensure quality code, allow time for testing,  and allow for any unforeseen problems that could occur. 


## Grant requested (DAI):
800 DAI


## Ethereum Address:
0x3D6087EbC73fb4f6d961a42076fA43A0Ae4e425c
