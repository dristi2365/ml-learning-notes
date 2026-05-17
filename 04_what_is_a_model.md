# What is a Model?

A model is the output of training — it's what the computer 
has learned after studying the training data.

## Simple analogy:
A model is like an experienced doctor. The doctor has seen 
thousands of patients (training data) and learned patterns. 
Now when a new patient comes in, the doctor uses that 
experience (the model) to make a prediction.

## Training vs Inference:
- Training — the model is learning (slow, needs lots of data)
- Inference — the model is making predictions using what it learned (fast)

## Real example:
In the padel project, YOLO was already trained by Ultralytics 
on millions of images. When we ran our code we were only doing 
inference — using the already trained model to detect players.
We never trained anything ourselves.

## The model file:
yolov8n.pt IS the model. All that learning stored in one file.
That's why you can't open it like a normal text file.
