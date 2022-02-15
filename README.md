# SQL 
## Case Study 
Health Analytics Mini Case Study

We’ve just received an urgent request from the General Manager of Analytics at Health Co requesting our assistance with their analysis of the health.user_logs dataset.

The Health Co analytics team have shared with us their SQL script - they unfortunately ran into a few bugs that they couldn’t fix!

We’ve been asked to quickly debug their SQL script and use the resulting query outputs to quickly answer a few questions that the GM has requested for a board meeting about their active users.


1 . How many unique users exist in the logs dataset? 
 <details>
<summary><b>ANSWER</b></summary>
    
    SELECT COUNT (DISTINCT ID)
    FROM health.user_logs

</details>

2 . How many total measurements do we have per user on average?
<details>
<summary><b>ANSWER</b></summary>

    SELECT id,
    COUNT(DISTINCT measure) as unique_measures
    FROM health.user_logs


</details>

