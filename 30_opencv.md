# OpenCV

OpenCV (Open Source Computer Vision Library) is a library 
that provides tools for working with images and videos 
in code - particularly Python.

## What it lets you do:
- Open and read video files frame by frame
- Read, resize, and manipulate images
- Draw shapes, text, and annotations on images/frames
- Apply filters, transformations, color conversions
- Save processed images or videos

## Why it's useful:
A video is just a sequence of images played quickly 
(e.g. 25-30 frames per second). OpenCV lets you treat 
a video as a series of individual images - read one, 
process it, move to the next.

## Common operations:
```python
import cv2

# Open a video
cap = cv2.VideoCapture("video.mp4")

# Read a frame
ret, frame = cap.read()

# Draw a rectangle
cv2.rectangle(frame, (x1, y1), (x2, y2), (0, 255, 0), 2)

# Add text
cv2.putText(frame, "Label", (x, y), 
             cv2.FONT_HERSHEY_SIMPLEX, 0.6, (0, 255, 0), 2)

# Save output video
out = cv2.VideoWriter("output.mp4", 
                       cv2.VideoWriter_fourcc(*"mp4v"), 
                       fps, (width, height))
out.write(frame)

# Release resources
cap.release()
out.release()
```

## Real world uses:
- Preprocessing images/video for ML models
- Drawing detection results (bounding boxes, labels)
- Video analysis applications
- Image filtering and enhancement
