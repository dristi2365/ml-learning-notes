# What is a Model?

A model is the output of training — it's what a machine 
has learned after studying data.

## Simple analogy:
Think of a model like an experienced doctor. After seeing 
thousands of patients over the years, the doctor recognizes 
patterns — certain symptoms point to certain conditions. 
A ML model works the same way. After studying thousands 
of examples it learns to recognize patterns and make 
predictions on its own.

## Training vs Inference:
- Training — the model is learning from data. 
  Slow, needs lots of examples.
- Inference — the model uses what it learned to make 
  predictions on new unseen data. Fast.

## Simple example:
Imagine training a model on thousands of emails labeled 
spam or not spam. After training it learns what spam looks 
like. Now give it a brand new email it has never seen — 
it predicts spam or not spam instantly. That's inference.

## The model file:
A trained model can be saved as a file. All that learning — 
millions of parameters and weights — stored in one place. 
This is why model files can be hundreds of megabytes in size 
and can't be opened like a normal text file. They're not 
meant to be read by humans, only used by code.
