# Named Entity Recognition

This is 1 task of the 2 tasks that were assigned to me by [WideBot](https://widebot.net/)<br>
I started the task by conducting a simple EDA to learn some facts about the data that I'll be working with and here is the most important stuff:<br>
1- the data is about 5,030 sentences and 22,525 words with only 2,523 unique words.<br>
2- the data has 13 unique labels with the label "x" representing about 86% of the total labels.<br>
3- there are no missing values in the dataset.<br>

The main thing that I'm concerned with for this task is the embeddings, a good word embedding model can help a lot with getting a good NER, but training a nice word embedding model takes a lot of data and computational power, I'm going to go initially with TF-IDF until I figure out a better solution.

I actually found a really nice solution for the embedding problem, thanks to **Pytorch** -I really love that framework :)-, Pytorch has a layer that's called `nn.Embedding` which is optimized as part of the training task. Consequently, after training, I should have embeddings that are specific to my task rather than generic embeddings that generate a more general representation which can be more or less useful but you know, compared to TF-IDF or the random mapping that I tried first :), I think that this would be a better solution -I'm going to try and compare them at the end in some nice table-, you can look at the whole discussion about `nn.Embedding` and how does it work [here](https://discuss.pytorch.org/t/how-does-nn-embedding-work/88518).

I take it back, actually, the hardest thing isn't finding the right word representation, the hardest thing is the fact that my whole city now has a wi-fi issue!


## Nice Tutriols:
1- [The Secret to Improved NLP: An In-Depth Look at the nn.Embedding Layer in PyTorch](http://webcache.googleusercontent.com/search?q=cache:https://towardsdatascience.com/the-secret-to-improved-nlp-an-in-depth-look-at-the-nn-embedding-layer-in-pytorch-6e901e193e16&strip=0&vwsrc=1&referer=medium-parser)<br>
2- [Essentials of Deep Learning: Introduction to Long Short Term Memory](https://www.analyticsvidhya.com/blog/2017/12/fundamentals-of-deep-learning-introduction-to-lstm/)
