# BERT_based_Sequence_Prediction
This BERT based Algorithm that I implemented in PyTorch is useful for predicting the order of sentences. For example, let's say we have three sentences:
1. He ate his lunch.
2. He closed his lunchbox.
3. Joe opened his lunchbox.

The order in which we have been provided the sentences is - 1,2,3 where as the actual order is 3,1,2. 
By training a BERT NextSentencePrediction algorithm with several examples from the training dataset, I could obtain a mean Spearman's rank correlation coefficient of 0.78 with this model on a test datset of 30000 paragraphs containing 6 sentences each, meaning 4 out of 5 paragraphs were being ordered corrrectly by the algorithm. 

Please get in touch with me to get the dataset (train.pkl and test.pkl) as they are large and I could not upload them here. 
Once you run this algorithm (it took ~ 3 hours on my 8GB RTX 2070 GPU), you will get an output file sentence_order that will contain the predicted order for the test sentences. I have included a sample sentence_order file in this repo. 


