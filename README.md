# To-Be-or-Not-To-Be

By Isaac Wu and Felix Stuart
October 6, 2026

We create an interesting embedder that predicts the distance between two tokens in the sentence
upon dot product.

E.g. for ["the", "brown", "dog"], the distance between "the" and "dog" is 2, so the embedder should be designed such that E("the") dot E("dog") = 2, where E is the embedding matrix and "the" and "dog" represent their one-hot encoded vectors.

Then, for prediction, we take the weighted average (with trained weighting) of the embeddings of the past window of words (window size of 8) and then put that vector into a feed-forward neural network to predict the next token.

Sample generation: what is thy seat of grief, when thou wouldst not speak no more to forget to hear the stars, and i am like high abroad and to hide his foot in sin.
what is the news?-- look'd upon a care, the people that thou, marcius: then, i must confess of hereford and henry's death, that he hath love in a wast, and he is born.
and my wrath of men.