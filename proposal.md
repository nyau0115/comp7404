
# Natural Language Processing - Question Answering System

We are Group P. Our proposal is to implement a question answering system by using the dataset from Wikipedia allowing user to input a question get a relevant answer from the dataset.

### Natural Language Processing

Natural Language Processing (NLP) is a study focusing on how computer understand, process and analysis natural language in a useful way. It is allow the computer to relay the human language and find out the pattern, feature and knowledge.

### Question Answering System

Question Answering System (QAS) retrieves information from a input dataset and output an relevant answer. It is a task of NLP and mainly focused on factoid questions which is simple and factual expression.

# Methodology

We propose to implement the QAS using Dynamic Memory Network (DMN). DMN is a neural network that can solve general QA task with the benefit of its memory system.

## Neural Network Architecture

### Dynamic Memory Network (DMN)

The QAS will be implemented with DMN because it a mature network for common factoid question answering task.

Below is the overview of DMN

![alt text](https://github.com/nyau0115/comp7404/blob/master/Overview%20of%20DMN%20modules.png?raw=true "Overview of DMN modules")

DMN is composed by four main model components which are input module, question module, episodic memory module and answer module.

![alt text](https://github.com/nyau0115/comp7404/blob/master/Question%20from%20the%20bAbI%20tasks.png?raw=true "Overview of DMN modules")
#### Input module

Input module is a Gated Recurrent Unit (GRU) which is a recurrent unit that running on the sequence of word vectors. It is used to compute the hidden state of every words.

## Data

### bAbI tasks

bAbl tasks is a research from Facebook providing a total of 40000 questions samples for training and testing.

Below Figure is some samples of bAbl tasks

![alt text](https://github.com/nyau0115/comp7404/blob/master/bAbl%20task.png?raw=true "Overview of DMN modules")

# Demo

The application is proposed to host and train in AWS as a Server with a Web client allowing user to input question to get an answer.

