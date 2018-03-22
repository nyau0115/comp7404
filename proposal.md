# Natural Language Processing - Question Answering System

We are Group P. For the presentation we intend to focus on Dynamic Memory Network, which is a machine learning technique useful for natural language processing.  We will illustrate the concept by implementing a question answering system with the dataset from Wikipedia to allow users to input a question and get a relevant answer from the dataset. 

### Natural Language Processing
Natural Language Processing (NLP) is a study focusing on enabling computers to understand, process and analyze natural language in a useful way. It allows the computer to relay the human language and find out the pattern, feature and knowledge.

### Question Answering System

Question Answering System (QAS) retrieves information from an input dataset and output a relevant answer. It is a task of NLP and mainly focused on factoid questions which is simple and factual expression.


# Methodology

We propose to implement the QAS using Dynamic Memory Network (DMN). DMN is a neural network that can solve general QA task with the benefit of its memory system.

## Neural Network Architecture

### Dynamic Memory Network (DMN)

The QAS will be implemented with DMN because it is a mature network for common factoid question answering task.   

Below is the overview of DMN

![alt text](https://github.com/nyau0115/comp7404/blob/master/Overview%20of%20DMN%20modules.png?raw=true "Overview of DMN modules")

DMN is composed by four main model components which are input module, question module, episodic memory module and answer module. 


![alt text](https://github.com/nyau0115/comp7404/blob/master/Question%20from%20the%20bAbI%20tasks.png?raw=true "Overview of DMN modules")

#### Input module
Input module is a Gated Recurrent Unit (GRU) which is a recurrent unit that runs on the sequence of word vectors. It is used to compute the hidden state of every word.

## Data

### bAbI tasks
bAbl tasks is a research from Facebook providing a total of 40000 questions samples for training and testing. 

Below Figure shows some samples of bAbl tasks 
![alt text](https://github.com/nyau0115/comp7404/blob/master/bAbl%20task.png?raw=true "Overview of DMN modules")

# Demo

The application is proposed to host and train in AWS as a Server with a Web client allowing user to input a question and get an answer.
