# Named Entity Recognition

This is 1 task of the 2 tasks that were assigned to me by [WideBot](https://widebot.net/)<br>
I started the task by conducting a simple EDA to learn some facts about the data that I'll be working with and here is the most important stuff:<br>
1- the data is about 5,030 sentences and 22,525 words with only 2,523 unique words.<br>
2- the data has 13 unique labels with the label "x" representing about 86% of the total labels.<br>
3- there are no missing values in the dataset.<br>

The main thing that I'm concerned with for this task is actually the embedding, training a nice word embedding model takes a lot of data and computational power, I'm going to go initially with TF-IDF until I figure out a better solution.
