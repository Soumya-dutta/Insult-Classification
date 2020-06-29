# Insult-Classification

Repository contains code for classifying text as insult or not insult. This was part of a hackathon that was held in IBM. Standard techniques for insult(sentiment) classification is used. Some highlights of the approach are as follows:

- **GLoVE** vectors are used for embedding the sentences
- A special technique that was used for this competition was both **post-padding** and **pre-padding**
- After the sequences are created the vectors are passed to **BiDirectional LSTM** and then **attention** block separately for post-padded and pre-padded sequences
- After the output from attention blocks they are **concatenated, flattened** and passed into a **sigmoid** layer for the result

# Results
A rank of 2 was achieved out of 10 teams. The metric provided by the hackathon organizers was 36976 on the test set.
