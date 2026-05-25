# Neural Networks

A neural network is a system loosely inspired by the human 
brain. Nodes are connected in layers and learn by adjusting 
connections based on how wrong their predictions are.

## Simple analogy:
Learning to ride a bike — you fall, your brain notes what 
went wrong, you adjust, repeat until perfect. A neural 
network learns the same way.

## Structure — Three types of layers:

**Input Layer:**
Receives raw data. Each feature becomes one input node.
Example: pixel values of an image, word frequencies in text.

**Hidden Layers:**
Where learning happens. Each layer learns increasingly 
complex patterns.
- Layer 1 might learn simple edges in an image
- Layer 2 might learn shapes from those edges  
- Layer 3 might learn faces from those shapes
More hidden layers = more complex patterns learned.

**Output Layer:**
Gives the final answer.
Example: Cat or Dog, Spam or Not Spam.

## How it learns — Backpropagation:
1. Forward Pass — data goes through all layers, 
   network makes a prediction
2. Calculate Error — compare prediction to actual answer
3. Backward Pass — error travels backward, each connection 
   adjusts slightly to reduce error next time
4. Repeat thousands of times until accurate

Like studying for an exam — attempt, check answer, 
understand what went wrong, improve. Repeat.

## Weights:
Every connection between nodes has a weight — controls 
how much influence one node has on the next.
Learning = adjusting these weights.
Like volume knobs — turned up or down until the right 
combination produces correct predictions.

## Deep Learning:
A neural network with many hidden layers.
More layers = can learn more complex patterns.
YOLO uses a deep neural network.

## Types of Neural Networks:

**CNN — Convolutional Neural Network:**
Specialized for images. Scans images in small patches.
Used in face recognition, object detection.

**RNN — Recurrent Neural Network:**
Specialized for sequences — text, speech, time series.
Has memory of previous inputs.
Used in language translation, speech recognition.

**Transformer:**
Most modern architecture. Powers ChatGPT and most 
modern AI. Extremely good at understanding context.

## Advantages:
- Can learn extremely complex patterns
- Works incredibly well for images, text and audio
- Improves with more data

## Disadvantages:
- Needs a lot of data to train well
- Very slow and expensive to train
- Hard to interpret — often called a black box
- Easy to overfit without careful tuning

## Real world examples:
- Face recognition on your phone
- Voice assistants like Siri and Alexa
- ChatGPT and other language models
- Self driving cars
- Medical image diagnosis
- YOLO object detection
