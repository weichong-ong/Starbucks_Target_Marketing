## Project Overview
The case we discuss here is a real-life marketing strategy study based on the simulated data set that mimics customer behaviour on the Starbucks rewards mobile app. The datasets used in the project are the simulated data about how people make purchasing decisions and how those decisions are influenced by promotional offers. The main task of this project is to combine transaction, demographic and offer data to determine which demographic groups respond best to which offer type and how best to present each type of offer. In the last part of this project, a classification model was built to predict whether or not someone will respond to an offer, as it allows Starbucks to maximise the profit of the next marketing campaign by sending the right offers to the the right customers.

## Data Set
The data is contained in three files:

* portfolio.json - containing offer ids and meta data about each offer (duration, type, etc.)
* profile.json - demographic data for each customer
* transcript.json - records for transactions, offers received, offers viewed, and offers completed

Here is the schema and explanation of each variable in the files:

**portfolio.json**
* id (string) - offer id
* difficulty (int) - minimum required spend to complete an offer
* reward (int) - reward given for completing an offer
* duration (int) - time for offer to be open, in days
* channels (list of strings)

**profile.json**
* age (int) - age of the customer 
* became_member_on (int) - date when customer created an app account
* gender (str) - gender of the customer (note some entries contain 'O' for other rather than M or F)
* id (str) - customer id
* income (float) - customer's income

**transcript.json**
* event (str) - record description (ie transaction, offer received, offer viewed, etc.)
* person (str) - customer id
* time (int) - time in hours since start of test. The data begins at time t=0
* value - (dict of strings) - either an offer id or transaction amount depending on the record

## Code and Resources
**Python Version:** 3.8

**Packages:** Pandas, Numpy, Matplotlib(Version 3.4.1), Seaborn, Sklearn

**Medium Blog Post:** [Target Marketing on Starbucks Rewards Mobile App](https://eden-ong.medium.com/target-marketing-on-starbucks-rewards-mobile-app-77a49afedeb3)


## Results
After all the analyse and visualizations, I can conclude that
- Women respond much better than men
- The best offer is offer 7: Buy 10 dollars get 2 dollars rewards within 10 days, sent via email, web, mobile and social
- Informational offer works better among young people
- Mobile and social advertising play an important role in getting positive response of the customers.