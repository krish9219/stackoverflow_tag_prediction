# Stackoverflow Tag Prediction #

If you are from Programming background you might aware of StackOverFlow. Many programmers asks their questions to get answers from another well know friend. All these questions will have some Title and Body. Have you ever wondered how StackOverFlow give Tags to the questions automatically based on the Title and Body of the question?

Well let us find how it works using Deep Learning Model (RNN with LSTM).

## Problem Statement ##
Predict the tags ( keywords, topics etc.), given only the question text and its title.

### Data ###

Data contains 8 fields in which we consider mainly 4 as believing these to be more valid to get better results

Id - Unique identifier for each question
Title - The question’s title
Body - The body of the question
Tags - The tags associated with the question

### Type of Machine Learning Problem ###

It is a multi-label classification problem.

In Multi-label Classification, multiple labels (in this problem its tags) may be assigned to each observation( here say questions) and there is no rule on how many of the classes the instance can be assigned to.

A question on Stackoverflow might be about any of C, C++, JAVA, Python, Regex, R Programming, .net or none of these.

### Performance metric ###

Using Machine Learning Algorithms can be easy to find metrics like Precision, Recall, F1 Score etc. When using DL models its bit complicate to show these metrics and requires bit more complex code too. In order to make it simple and understandable i'm considering metrics called 'Val_loss'.

### Tags analysis ###

1. Maximum number of tags per question: 5
2. Minimum number of tags per question: 1
3. Questions with 3 tags appeared more in number.

