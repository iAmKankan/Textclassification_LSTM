## Text Classification Using LSTM
![deep](https://user-images.githubusercontent.com/12748752/181097747-f97a41d2-ebab-4295-8dae-fac47563a251.png)

## PROBLEM STAEMENT
![deep](https://user-images.githubusercontent.com/12748752/181097747-f97a41d2-ebab-4295-8dae-fac47563a251.png)
In this project we will be building a text classifier using **LSTM** and **wor2vec**.
## DESCRIPTION OVERVIEW
![deep](https://user-images.githubusercontent.com/12748752/181097747-f97a41d2-ebab-4295-8dae-fac47563a251.png)
Text classification  is the task of assigning a set of predefined categories to free-text. Text classifiers can be used to organize, structure, and categorize pretty much anything. For example, new articles can be organized by topics, support tickets can be organized by urgency, chat conversations can be organized by language, brand mentions can be organized by sentiment, and so on.
There are many approaches to automatic text classification, which can be grouped into three different types of systems:
*	Rule-based systems
*	Machine Learning based systems
*	Hybrid systems

Deep learning algorithms such as **Word2vec** and **Glove** are also used in order to obtain better vector representations for words and improve the accuracy of classifiers trained with traditional machine learning algorithms.
Few typical applications of text classification technology including all of the following:
*	Social media monitoring.
*	Brand monitoring.
*	Customer service.
*	Voice of customer.

## TECHNOLOGY USE
![deep](https://user-images.githubusercontent.com/12748752/181097747-f97a41d2-ebab-4295-8dae-fac47563a251.png)
Here we will be using  Anaconda Python 3.6 , Pytorch 1.4 with GPU support CUDA 10 with CuDNN 10.

## INSTALLATION
![deep](https://user-images.githubusercontent.com/12748752/181097747-f97a41d2-ebab-4295-8dae-fac47563a251.png)
Installation of this project is pretty easy. Please do follow the following steps to create a virtual environment and then install the necessary packages in the following environment.

**In Pycharm it’s easy** 

1. Create a new project.
2. Navigate to the directory of the project
3. Select the option to create a new new virtual environment using conda with python3.6
4. Finally create the project using used resources.
5. After the project has been created, install the necessary packages from **requirements.txt** file using the command _`pip install -r requirements.txt`_


**In Conda also it’s easy**

1. Create a new virtual environment using the command
    _`conda create -n your_env_name python=3.6`_
2. Navigate to the project directory.
3. Install the necessary packages from requirements.txt file using the command _`pip install -r requirements.txt`_

## WORKFLOW DIAGRAM
![deep](https://user-images.githubusercontent.com/12748752/181097747-f97a41d2-ebab-4295-8dae-fac47563a251.png)

<p align="center">
  <img src="https://user-images.githubusercontent.com/12748752/211185117-65f44c19-0184-4853-ad68-99a14aaa0299.png" width=60%/>
</p>

## IMPLEMENTATION
![deep](https://user-images.githubusercontent.com/12748752/181097747-f97a41d2-ebab-4295-8dae-fac47563a251.png)

### 1. Project Directory
![light](https://user-images.githubusercontent.com/12748752/181097751-9be22081-c630-4756-9ea8-2c27fdce6984.png)

<p align="center">
  <img src="https://user-images.githubusercontent.com/12748752/211185221-80ca074c-9b22-4b60-98c9-569c3329c780.png" width=60%/>
</p>

This is the complete folder stucture of the project.

### 2. preprocess.py
![light](https://user-images.githubusercontent.com/12748752/181097751-9be22081-c630-4756-9ea8-2c27fdce6984.png)
<p align="center">
  <img src="https://user-images.githubusercontent.com/12748752/211185286-937f9163-d0f1-4234-9339-2ad8e9af9e1d.png" width=60%/>
</p>

This file is used for data processing. It will create _train_preprocessed.pickle_ , _validation_preprocessed.pickle_ and _test_preprocessed.pickle_ files under **data folder**.

### 3. word_embedder_gensim.py
![light](https://user-images.githubusercontent.com/12748752/181097751-9be22081-c630-4756-9ea8-2c27fdce6984.png)

<p align="center">
  <img src="https://user-images.githubusercontent.com/12748752/211185342-115c702f-b3e6-4b7b-9273-a40c564e525a.png" width=60%/>
</p>

This file will training  the **Word2Vec** embeddings.

### 4. rnn_w2v.py
![light](https://user-images.githubusercontent.com/12748752/181097751-9be22081-c630-4756-9ea8-2c27fdce6984.png)

<p align="center">
  <img src="https://user-images.githubusercontent.com/12748752/211185370-deaac542-5915-4a79-bd5b-f094517d3928.png" width=60%/>
</p>

This file will train the LSTM network.

### 5. TextCategorizer.py
![light](https://user-images.githubusercontent.com/12748752/181097751-9be22081-c630-4756-9ea8-2c27fdce6984.png)

<p align="center">
  <img src="https://user-images.githubusercontent.com/12748752/211185390-f48f8e6a-3892-47ed-9be7-ac2c1aec1041.png" width=60%/>
</p>

This file will be used for prediction of any input text.



