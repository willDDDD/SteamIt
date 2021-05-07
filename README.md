# SteamIt

## Project Title: SteamIt
## Project Summary
Our application “steamit” is a website that provides game recommendations to users according to different aspects such as age, tag, genres. We also record the search history of each user to improve our accuracy of recommendation.
## Main parts of our website
There are three main parts. First part is game name search, users can enter the Game name to get the platform requirement, developer, and price, also the frequencies that each game has been searched will be recorded in our GCP. Second part is the user login/game recommend part, user can use their name, their age, and the tag they want to search as one record to insert into our database. We will see the persons have same name and same age as the same user. So, if you insert two records with same name and same age, the second insert will be denied and the first insert will be kept, if you want to change your tags, you can only update your previous record. After inserting the user information, our database will recommend several games under the tag user choose based on our advanced query (depend on the positive ratings and average play time). At the same time, all the records that insert into our database will be recorded, and it does not matter whether you delete or update your records in some time, all the insert information will be recorded. The Third part is the store procedure part. Our store procedure will return three history tables, which are gamehistory, taghistory and agehistory, all this history tables are based on the information that users searched or inserted in our APP before.
## What different?
Our application provides a new way of recommending games. Normal search engine would only return the result related to user’s already bought game, while our application provides a new way of providing a list of games that people who at the same or nearby age have once searched or were interested in. We also provide another game list according to the search history which offers a different view.
## Raw Data references
We download the raw datasets from Kaggle.com and use Jupyter notebooks to process raw data in order to get proper form to fit in Google Cloud platform.

## Authors and acknowledgment
Xiuhao Ding - Front/backend integration, dataflow integration, Processing raw data, Database algorithm.

Yu Yang - Processing raw data, Analyze indexing, Front/backend integration.

Fangyi Zhang - Front page design, Video

Zongxian Feng - Deploying our React App to Google Cloud Platform, Processing raw data, Front/backend integration, Assist other team members.