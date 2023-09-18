# podscribe-assessment

## Challenge 1 : SQL

### SQL Query to get data from last two months

```
SELECT *
FROM thirdauth_episodeadvertiser
WHERE created_at >= NOW() - INTERVAL '2 months'
```
and 
```
SELECT *
FROM thirdauth_advertiser
WHERE created_at >= NOW() - INTERVAL '2 months'
```
The data generated from the above queries can be found in the files `thirdauth_episodeadvertiser.csv` and `thirdauth_advertiser.csv` respectively.
    
The answers to the following questions from the txt file are in the file `sqlchallenge.ipynb`


## Challenge 2 : Prompt Engineering

### How would you refine this prompt to improve the output? 

There is a lot of ambiguity in the prompt. I would ask for a short clarification on why exactly the AI categorizes the ad as host_read or producer_read. Also why it thinks it is Direct Response or Brand Awareness.

### How would you find tune it? 

I would try to find out what the AI is looking for in the ad to categorize it as host_read or producer_read. I would also try to find out what the AI is looking for to categorize it as Direct Response or Brand Awareness.

### Explain how you would train a model or refind and test a prompt like this to further improve Podscribe's automated ad scoring feature?

As a first step, to train the model I would use more manually trained data.

