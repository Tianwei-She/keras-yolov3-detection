# YOLOv3-Detection

This repo implements object detection on one single image or one video, using a pretrained YOLOv3 model. The output is saved in an image/video file with detected bounding boxes plotted.

The code is mostly copied from the following 2 repos with minor modifications
* [qqwweee/keras-yolo3](https://github.com/qqwweee/keras-yolo3)
* [experiencor/keras-yolo3](https://github.com/experiencor/keras-yolo3)

```
wget https://pjreddie.com/media/files/yolov3.weights -P PATH/TO/WEIGHTS_FOLDER
python convert.py data/yolov3.cfg PATH/TO/WEIGHTS_FOLDER/yolov3.weights PATH/TO/WEIGHTS_FOLDER/yolov3.h5
# Image
python detect.py --model_path PATH/TO/WEIGHTS_FOLDER/yolov3.h5 --input_path PATH/TO/INPUT/IMAGE --output_path PATH/TO/OUTPUT/IMAGE
# Video
python detect.py --video --model_path PATH/TO/WEIGHTS_FOLDER/yolov3.h5 --input_path PATH/TO/INPUT/VIDEO --output_path PATH/TO/OUTPUT/VIDEO
```
