## Image Segmentation

Image segmentation is the task of partitioning an image into meaningful regions — 
teaching a model to identify not just **what** objects are present, but exactly 
**which pixels** belong to each object.

Unlike object detection (which draws bounding boxes around objects), segmentation 
produces pixel-level masks for much finer understanding.

### Types

**Semantic Segmentation**
Labels every pixel with a class (e.g. "road", "sky", "person") but doesn't 
distinguish between individual instances of the same class.

**Instance Segmentation**
Goes further — distinguishes between individual objects of the same class.
e.g. Person 1, Person 2, Person 3 are all labeled separately.

**Panoptic Segmentation**
Combines both — labels every pixel AND distinguishes instances.

### Common Models
- **U-Net** — popular in medical imaging
- **Mask R-CNN** — instance segmentation
- **SAM (Segment Anything Model)** — Meta's foundation model for segmentation

### Real World Uses
- Medical imaging (tumor detection)
- Autonomous driving (road, pedestrian, lane detection)
- Satellite imagery analysis
