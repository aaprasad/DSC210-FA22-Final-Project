# DSC210-FA22-Final-Project


Code base for DSC 210 Fall 22 Final Project on NonNegative Factorization


This project compares topic modelling techniques on Headlines dataset and Presidential speech dataset. In particular we are using LDA and NMF on both datasets and comparing the results.  
Here you can know more on the datasets.
https://www.kaggle.com/datasets/littleotter/united-states-presidential-speeches
https://www.kaggle.com/datasets/therohk/million-headlines

More details and results of this project can be found at: (Add viewer notion document link here)
https://docs.google.com/presentation/d/1iEcSMdsYv4pO6Yf69snHWFZqtMSQovcz0dQbwrk0AaU/edit?usp=sharing


## Code-Base Structure
We have 4 notebooks applying a model on a dataset. 
LDA-Headlines dataset
NMF-Headlines dataset
LDA-Presidential speech dataset
NMF-Presidential speech dataset

## Instructions to run notebook that runs LDA on Headlines
Running on colab:

Download the dataset from the link given above and upload it to your google drive's root folder.
There is a cell in the notebook to connect to google drive which will ask the permission to connect to drive.
After that you can just sequentially run all the cells and get the results.
Note the cell that trains the lda models takes a lot of time to run so keep some patience.

Running on local:

Download the dataset from the link given above and upload it to your google drive's root folder.
You do not need to run the cell that connects to google drive.
Change the path to read the dataset to you local machines current path.
After that you can just sequentially run all the cells and get the results.
Note the cell that trains the lda models takes a lot of time to run so keep some patience.

## Results LDA Headlines:

![10_topics](https://user-images.githubusercontent.com/44918113/205547721-1c6e236b-1a2e-49e8-93f0-7a555426302c.png)


These are the top 10 words of the top 10 topics from the model trained with 10 topics. The coherence score is pretty low for a model with 10 topics as the dataset is pretty huge. These topics do not make much sense.

![200_topics](https://user-images.githubusercontent.com/44918113/205547759-8b5c6fbf-8dbd-4cf4-99c1-099ea81eebd7.png)


These are the top 10 words of the top 10 topics from the model trained with 200 topics. We got the best coherence score from this model and it shows as the topics make much more sense than before. 

![coherence topics](https://user-images.githubusercontent.com/44918113/205547787-430680e6-4f72-4f63-88d5-d85551f6ec45.png)


This graph is the graph of the coherence score for a number of topics. We got the best coherence score for this model with 200 topics.

![memory:topics](https://user-images.githubusercontent.com/44918113/205547801-c88ce79f-8fa7-434b-b1d8-55b2989b664b.png)


This graph is the graph of memory for a number of topics. The memory usage to train this model increases with the number of topics.

![topics time](https://user-images.githubusercontent.com/44918113/205547867-ac23f374-2052-490b-bd90-50137ad72d69.png)


This graph is the graph of training time for a number of topics. The training time to train this model increases with the number of topics.

![sentence_topic_10](https://user-images.githubusercontent.com/44918113/205547895-d099033f-69c7-40f6-804c-8c0582274ccd.png)



We classified sentences using the model trained with 20 topics into topics. This classification does not make much sense as the coherence score for the model trained with 20 topics was pretty bad. 

![sentence_topic_200](https://user-images.githubusercontent.com/44918113/205547919-51713dc7-c795-49f2-b2a3-5bf224bbbc02.png)


We classified sentences using the model trained with 200 topics into topics. The classification makes much more sense as the coherence score was the maximum with a model trained with 200 topics.

