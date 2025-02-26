# 1 Introduction to Machine Learning

## 1.1. Machine Learning

The main idea behind machine learning is learning from examples: we prepare a dataset with examples, and a machine learning system “learns” from this dataset. In other words, we give the system the input and the desired output, and the system tries to figure out how to do the conversion automatically, without asking a human.

We can collect a dataset with descriptions of cars and their prices, for example. Then we provide a machine learning model with this dataset and “teach” it by showing it cars and their prices. This process is called training or sometimes fitting.

When training is done, we can use the model by asking it to predict car prices that we don’t know yet.

All we need for machine learning is a dataset in which for each input item (a car) we have the desired output (the price).

The difference between a traditional software system and a machine learning system. In traditional software engineering, we do all the work, whereas in machine learning, we delegate pattern discovery to a machine.

### 1.1.1. Machine Learning vs. Rule-Based Systems

In machine learning, we typically don't attempt to extract patterns manually. Instead, we delegate the tasks to statistical methods.

If something changes in the future, we don't have to revisit all the patterns manually and try to reorganize them. Instead we use only the most recent data and replace the old model with the fresh one.

### 1.1.2. When Machine Learning Isn't Helpful

Machine learning isn't always helpful or needed. For simple tasks, rules can often work well. In some cases, such as theoe wuthout a dataset, it isn't possible to perform machine learning.

### 1.1.3. Supervised machine learning

Supervised machine learning is when we provide the model with features and the target variable, and it figures out how to use these features to arrive at the target. We supervise or teach the model by showing it examples.

The main types of supervised learning problems are:

1. Regression
2. Classification
3. Ranking

## 1.2. Machine learning process

Accordiung to CRISP-DM, the machine learning process has six steps:

1. Business understanding

- try to identify the problem
- understand how you can solve it
- decide whether machine learning will be a useful tool for solving it

2. Data understanding

- analyze datasets and decide whether you need to collect more data

3. Data preparation

- transform the data into a tabular form that you can use as input for a machine learning model

4. Modeling

- you train a model

5. Evaluation

- you evaluate the model to see if it solves the original business problem and maesure its success at doing that

6. Deployment

- deploy the model to the production environment

## 1.3. Modeling and model validation

Setting the calidation process is the most important step in machine learning. Without it, there's no reliable way to know whether the model we've just trained is good, useless, or even harmful.

The process of selecting the best model and the best parameters for the model is called model selection

Model selection:

1. Split the data into training, validation, and testing parts
2. Train each model first on the training part and then evaluate it on validation
3. Each time we train a different model, we record the evaluation results using the validation part
4. At the end, determine which model is the best and test it on the test dataset
