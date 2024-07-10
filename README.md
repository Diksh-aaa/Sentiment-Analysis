
# What is Sentiment Analysis

Sentiment analysis is the process of classifying whether a block of text is positive, negative, or neutral. The goal that Sentiment mining tries to gain is to be analysed people’s opinions in a way that can help businesses expand. It focuses not only on polarity (positive, negative & neutral) but also on emotions (happy, sad, angry, etc.). It uses various Natural Language Processing algorithms such as Rule-based, Automatic, and Hybrid.

# Why is Sentiment Analysis important?

- Customer Feedback Analysis: Businesses can analyze customer reviews, comments, and feedback to understand the sentiment behind them helping in identifying areas for improvement and addressing customer concerns, ultimately enhancing customer satisfaction.
- Brand Reputation Management: Sentiment analysis allows businesses to monitor their brand reputation in real-time.
- By tracking mentions and sentiments on social media, review platforms, and other online channels, companies can respond promptly to both positive and negative sentiments, mitigating potential damage to their brand.
- Product Development and Innovation: Understanding customer sentiment helps identify features and aspects of their products or services that are well-received or need improvement. This information is invaluable for product development and innovation, enabling companies to align their offerings with customer preferences.
- Competitor Analysis: Sentiment Analysis can be used to compare the sentiment around a company’s products or services with those of competitors.
- Businesses identify their strengths and weaknesses relative to competitors, allowing for strategic decision-making.
- Marketing Campaign Effectiveness
- Businesses can evaluate the success of their marketing campaigns by analyzing the sentiment of online discussions and social media mentions.
- Positive sentiment indicates that the campaign is resonating with the target audience, while negative sentiment may signal the need for adjustments.

# BERT (Bidirectional Representation for Transformers)

Bidirectional Encoder Representation for Transformer (BERT) is an NLP model developed by Google Research in 2018, after its inception it has achieved state-of-the-art accuracy on several NLP tasks. Transformer architecture has encoder and decoder stack, hence called encoder-decoder architecture whereas BERT is just an encoder stack of transformer architecture. There are two variants, BERT-base and BERT-large, which differ in architecture complexity. The base model has 12 layers in the encoder whereas the Large has 24 layers.

# BERT Tokenization

BERT tokenizer uses something known as sub word-based tokenization. Sub word-tokenization splits unknown words into smaller words or characters such that the model can derive some meaning from the tokens. For example ‘boys’ is divided into ‘boy’ and ‘s’. BERT uses word piece algorithm to generate the vocabulary. Word piece algorithm generates sub words based on the likelihood of characters occurring together.

- Input IDs – The input ids are often the only required parameters to be passed to the model as input. Token indices, numerical representations of tokens building the sequences that will be used as input by the model.
- Attention mask – Attention Mask is used to avoid performing attention on padding token indices. Mask value can be either 0 or 1, 1 for tokens that are NOT MASKED, 0 for MASKED tokens.
- Token type ids – It is used in use cases like sequence classification or question answering. As these require two different sequences to be encoded in the same input IDs. Special tokens, such as the classifier\[CLS\] and separator\[SEP\] tokens are used to separate the sequences.

# Training the BERT model for Sentiment Analysis

Now we can fine-tuning process using the ‘Keras’ API ‘model.fit’.

