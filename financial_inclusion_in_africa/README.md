
# Financial Inclusion in Africa
Knowledge/Pre-Qualification to AI Hack Tunisia 2019.  
competition website: [zindi.africa](http://zindi.africa/competitions/financial-inclusion-in-africa)

## Description
Financial Inclusion remains one of the main obstacles to economic and human development in Africa. For example, across Kenya, Rwanda, Tanzania, and Uganda only 9.1 million adults (or 13.9% of the adult population) have access to or use a commercial bank account.

Traditionally, access to bank accounts has been regarded as an indicator of financial inclusion. Despite the proliferation of mobile money in Africa, and the growth of innovative fintech solutions, banks still play a pivotal role in facilitating access to financial services. Access to bank accounts enable households to save and facilitate payments while also helping businesses build up their credit-worthiness and improve their access to other finance services. Therefore, access to bank accounts is an essential contributor to long-term economic growth.

The objective of this competition is to create a machine learning model to predict which individuals are most likely to have or use a bank account. The models and solutions developed can provide an indication of the state of financial inclusion in Kenya, Rwanda, Tanzania and Uganda, while providing insights into some of the key demographic factors that might drive individuals’ financial outcomes.

While this competition is open to all, registered participants of AI Hack Tunisia 2019 must complete this challenge to qualify for the main event which will take place in Tunis, Tunisia from Sep 20th to 22nd 2019

AI Hack Tunisia 2019 is organised by InstaDeep, with the support of Google and the Tunisian Ministère de l'Industrie et des PMEs (Ministry of Industry and SMEs).

## Rules
As this is a learning challenge, aside from the rules in the Zindi Terms of Use, no other particular rules apply.

We do, however, encourage all participants to share their code with Zindi, as well as on GitHub as a public good to the sector.

Note that there is **Public** and **Private Leaderboards**. The Public Leaderboard excludes approximately 50% of the test dataset. While the competition is open, the Public Leaderboard will rank the submitted solutions by the accuracy score they achieve. Upon close of the competition, the Private Leaderboard, which covers 100% of the test dataset, will be made public and will constitute the final ranking for the competition.

Maximum 10 solutions submitted per day.

We reserve the right to modify these rules at any time as necessary.

## Prizes
This competition is a pre-qualification challenge for AI Hack Tunisia 2019. Your score will be considered as part of your application to the event.

This competition is also open to all 'Zindians' as a learning competition. There are no prizes for this competition.

## Evaluation
The evaluation metric for this challenge will be the percentage of survey respondents for whom you predict the binary 'bank account' classification incorrectly.

Your submission file should look like:

| unique_id           |  bank_account  |
| ------------------- | -------------- |
| <string>            |    <number>    |
| uniqueid_1 x Kenya  |        1       |
| uniqueid_2 x Kenya  |        0       |
| uniqueid_3 x Kenya  |        1       |

## Timeline
Competition closes on 31 August 2019

Final submissions must be received by 11:59 PM GMT.

We plan to reopen this competition and leaderboard again later in the year.

We reserve the right to update the contest timeline if necessary.

## Financal Inclusion Survey Data
The main dataset contains demographic information and what financial services are used by approximately 33,610 individuals across East Africa. This data was extracted from various Finscope surveys ranging from 2016 to 2018, and more information about these surveys can be found here:

* FinAccess Kenya 2018
* Finscope Rwanda 2016
* Finscope Tanzania 2017
* Finscope Uganda 2018

The data have been split between training and test sets. The test set contains all information about each individual except for whether the respondent has a bank account or not.

Your goal is to accurately predict the likelihood that an individual has a bank account or not, i.e. Yes = 1, No = 0.

### About the data

You are asked to make predictions for each unique id in the test dataset about the likelihood of the person having a bank account. You will train your model on 70% of the data and test your model on the final 30% of the data.

**Train.csv** is 70% of the data, across the four East African countries (i.e. Kenya, Rwanda, Tanzania, and Uganda)

**Test.csv** is 30% of the complete dataset across the East African countries.

**SubmissionSubmission.csv** is an example of what your submission file should look like. Note that the variable unique_id in the submission file is:

 uniqueid + " x " + country name
The order of the rows do not matter, but the names of the unique_id's must be correct. The column "bank_account" is your prediction of the likelihood of the user having a bank account

**VariableDefinitions.csv** is the full list of variables and their explanations.