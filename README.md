# Sentiment-analysis-with-tweets-about-cancer-misinformation
This notebook is part of my master's thesis.

The notebook of this repository is divided into two main parts. In the first part, the entailment recognition and sentiment classification models are inferred from previously mined tweets. In the second section, the code for an analysis and visualization of the classified sentiments is found.

It should be noted that the data mined from twitter as well as the keys to mine in the API are confidential. The entailment recognition model is also a private access model.

# Model Inference
 The entailment recognition model was used to filter cancer misinformation tweets. The texts of the tweets were compared to a series of mined hoaxes. With this step you want to eliminate noise and tweets that are not related to the disinformation tracked.

Next, two sentiment classification models were applied to the filtered tweets.
- Polarity model: This model can be found on the Hugging face hub under the name "cardiffPLN/twitter-roberta-base-sentiment-latest". It is a model that was specifically fine-tuned to classify polarity in tweets. The model is able to classify the text between positive, neutral or negative
- Emotions model: This model was also fine-tuned specifically with tweets. It is able to classify the tweets between joy, optimism, sadness or anger. The model is available on Hugging Face under the name "cardiffnlp/twitter-roberta-base-emotion".

#Analysis
In the analysis, I carried out a comparison between the mined tweets and the filtered ones.
Then the polarity and emotions of the hoaxes were analyzed and visualized
