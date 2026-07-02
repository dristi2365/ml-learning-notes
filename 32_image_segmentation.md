# Image Segmentation
Image segmentation is the task of partitioning an image into meaningful regions 
or segments — essentially teaching a model to identify not just what objects are 
present, but exactly which pixels belong to each object.

Unlike object detection (which draws bounding boxes), segmentation produces 
pixel-level masks. There are two main types:
- Semantic segmentation: labels every pixel with a class (e.g. "road", "sky", "person")
- Instance segmentation: distinguishes between individual instances of the same class

Common models: U-Net (medical imaging), Mask R-CNN, SAM (Segment Anything by Meta)
