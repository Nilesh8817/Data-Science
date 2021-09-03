## Amazon fine food review - Sentiment analysis
<p>The analysis is to study Amazon food review from customers, and try to predict whether a review is positive or negative. The dataset contains more than 500K reviews with number of upvotes & total votes to those comments.</p>

<b>AIM</b>

<p>We are going to tackle an interesting natural language processing problem i.e. Sentiment Analysis. Our aim is to predict whether a review is positive or negative.</p>

### All the basic imports
![image](https://user-images.githubusercontent.com/81873172/131953557-9ab7f5d2-d7bb-4d60-85fe-13a4a45c0a06.png)

<b>First 5 columns of dataset to view data</b>

![02](https://user-images.githubusercontent.com/81873172/131954034-b0a939a3-627d-47df-ad1c-84fb71e8ed37.jpg)

## Preproccessing

**<li>Replacing the words</li>**

![04](https://user-images.githubusercontent.com/81873172/131954214-9a99b194-267d-4a53-a57c-8a3ffe2071b8.jpg)

**<li>Function to Removing Website links, HTML tags, converting words/sentences to lower case</li>**

![05](https://user-images.githubusercontent.com/81873172/131954386-88877ddc-79a5-4bf1-9f9a-78969110fda2.jpg)

**<li>Dataset after Preprocessing</li>**

![06](https://user-images.githubusercontent.com/81873172/131954544-f6940adb-9f84-4dbe-92c3-8601a0c7bc49.jpg)
![07](https://user-images.githubusercontent.com/81873172/131954580-4a0fc829-ab64-4361-a2d3-f782d50d0fb7.jpg)

**<li>Most Repeting words in Negative reviews(with the help of WordCloud)</li>**

![image](https://user-images.githubusercontent.com/81873172/131954848-8fda99bf-058f-4b09-a0a7-8831e6573744.png)

**<li>Most Repeting words in Positive reviews(with the help of WordCloud)</li>**

![image](https://user-images.githubusercontent.com/81873172/131954919-acc7afdb-6b9b-4ff7-8b96-f6ce2a2e476b.png)

**<li>Target column</li>**

![03](https://user-images.githubusercontent.com/81873172/131955001-91f9abd5-5f79-42c9-bdba-7509bab37acb.jpg)

**<li>Tokenization</li>**
<p>Tokenization is the process of tokenizing or splitting a string, text into a list of tokens. One can 
think of token as parts like a word is a token in a sentence, and a sentence is a token in a 
paragraph</p>
Applying Tokenization on training data.

![10](https://user-images.githubusercontent.com/81873172/131955100-b092e1df-b2f9-464b-9231-d0fa46c77425.jpg)

**<li>Neural Network</li>**

![11](https://user-images.githubusercontent.com/81873172/131955187-f3040ff9-f2e8-4460-a3c0-62e612bc2625.jpg)
![12](https://user-images.githubusercontent.com/81873172/131955212-da30a493-979a-41e5-a8fc-b35371c387be.jpg)

**SCORE**

![IMG_20210703_114503](https://user-images.githubusercontent.com/81873172/131955395-e7d5b6ca-ce62-4528-9f50-b40f1b6cbdf2.jpg)

**<li>After Performing various models we get good score with Bidirectional RNN with Multiple Layer</li>**

**<li>Bidirectional RNN with Multiple Layer</li>**

![image](https://user-images.githubusercontent.com/81873172/131955626-0b73ace4-9126-481c-8ce0-94760767ac4c.png)
![image](https://user-images.githubusercontent.com/81873172/131955798-e7f16015-98ff-4841-8be8-a45d12b897ca.png)

## Conclusion. 
 
**Step 1.** Remove/drop Unwanted column.

**Step 2.** Convert Score / Reviews 1 if score is > 3 else 0.

**Step 3.** Check if there is any website link or any HTML tag are present or not.

**Step 4.** Perform Preprocessing on Text column remove website links, stop words, etc.

**Step 5.** Plot image with word cloud to observe what words are repeated many times.

**Step 6.** Split data into train and test.

**Step 7.** Perform Tokenization on training data.

**Step 8.** Get the maximum length which is covered by 95% of data.

**Step 9.** Create Neural Network with Flatten and observer the score of testing data.

**Step 10.** After performing NN Perform RECURRENT NEURAL NETWORK (RNN), LONG SHORT-TERM MEMORY (LSTM), and GATED RECURRENT UNITS (GRU) and observe the score & try to improve the recall/score. 


## ALL OVER RESULT 
 
<p><b>In this Project I have perform almost all the model: With Neural Network we get accuracy score of 80% we perform RECURRENT NEURAL NETWORK (RNN), LONG SHORT-TERM MEMORY (LSTM), GATED RECURRENT UNITS (GRU) with single, multiple and Bidirectional Layer as well to improve the score & we get the Best score with Bidirectional RECURRENT NEURAL NETWORK (RNN) with Multiple layer of 85% of recall as well as 85% of accuracy.</b></p>

Presentation file:<br>

[Food Review](Sentiment Analysis on Food review.ipynb)
