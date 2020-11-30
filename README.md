# Starbucks-Offer-Recommendataion-Capstone
Data Scientist Nanodegree of Udacity

### Table of Contents

1. [Installation](#installation)
2. [Project Details](#motivation)
3. [Dataset Details](#files)
4. [Results](#results)
5. [Credits](#licensing)

## Installation <a name="installation"></a>

There should be no necessary libraries to run the code here beyond the Anaconda distribution of Python.  The code should run with no issues using Python versions 3.*.

## Project Details<a name="motivation"></a>

It is the Starbuck's Capstone Challenge of the Data Scientist Nanodegree in Udacity. 

We got the dataset from the program that creates the data simulates how people make purchasing decisions and how those decisions are influenced by promotional offers. 

We want to make a recommendation engine that recommends Starbucks which offer should be sent to a particular customer.

We are interested in checking which offer should be sent to a customer to influence them to purchase ?


## Data set details <a name="files"></a>

I have attached a notebook which has all the analysis in steps.  

This data set is a simplified version of the real Starbucks app because the underlying simulator only has one product whereas Starbucks actually sells dozens of products.

The data is contained in three files:
- `portfolio.json` - containing offer ids and meta data about each offer (duration, type, etc.)
- `profile.json` - demographic data for each customer
- `transcript.json` - records for transactions, offers received, offers viewed, and offers completed

Here is the schema and explanation of each variable in the files:

`portfolio.json`
- id (string) - offer id
- offer_type (string) - the type of offer ie BOGO, discount, informational
- difficulty (int) - the minimum required to spend to complete an offer
- reward (int) - the reward is given for completing an offer
- duration (int) - time for the offer to be open, in days
- channels (list of strings)

`profile.json`
- age (int) - age of the customer
- became_member_on (int) - the date when customer created an app account
- gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
- id (str) - customer id
- income (float) - customer's income

`transcript.json`
- event (str) - record description (ie transaction, offer received, offer viewed, etc.)
- person (str) - customer id
- time (int) - time in hours since the start of the test. The data begins at time t=0
- value - (dict of strings) - either an offer id or transaction amount depending on the record


## Results<a name="results"></a>

Results and detailed analysis has been published as an [article](https://vijay2035.medium.com/starbucks-challenge-d5a7aba7cb08).

## Credits<a name="licensing"></a>

Data and scenarios - Starbucks, Udacity