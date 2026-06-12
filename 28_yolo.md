# YOLO (You Only Look Once)

YOLO is a popular pretrained object detection model. 
It can identify objects in images and tell you exactly 
where they are by drawing bounding boxes.

## What makes it special - speed:
Unlike older models that scan an image multiple times in 
different regions, YOLO looks at the entire image just 
once and predicts all objects simultaneously. This makes 
it extremely fast - suitable for real time video processing.

## How it works (simplified):
1. Divides the image into a grid
2. For each grid cell, predicts:
   - Is there an object here?
   - What class is it? (person, car, ball, etc.)
   - Where exactly are its boundaries? (bounding box)
   - How confident is the prediction? (confidence score)
3. Combines all predictions into final detections

## Pretrained on COCO dataset:
YOLO models are commonly pretrained on the COCO dataset - 
80 object classes including person, car, dog, sports ball, 
chair, and more. Each class has a number (e.g. class 0 = person).

## Versions:
YOLO has had many versions (v3, v5, v8...) each improving 
speed and accuracy. Comes in different sizes - nano (n), 
small (s), medium (m), large (l) - trading off speed vs accuracy.

## Real world uses:
- Real time object detection in video
- Self driving cars
- Security and surveillance
- Sports analytics
- Retail (inventory tracking)
