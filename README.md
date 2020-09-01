# Object-Detection-with-YOLOv3
This project : <br />
1.Performs real-time object detection with YOLOv3  <br />
2.Uses OpenCV to manipulate video data <br />
3.Uses pre-trained models and COCO dataset to perform real-time and passive inference with/without a GPU <br />
4.Develops a simple command line application with Python for inference  which saves output as a .mp4 file(yolo_utils.py&yolo.py) <br />
<br />
Download pretrained yolov3 weights- $wget https://pjreddie.com/media/files/yolov3.weights  <br />
Download pretrained yolov3-tiny weights- $wget https://pjreddie.com/media/files/yolov3-tiny.weights <br />
Use darknet directory: git clone https://github.com/pjreddie/darknet<br />
for more info on darkset visit:https://pjreddie.com/darknet/yolo/ <br />
<br />
Note:Output sample image for yolov3 and yolov3 tiny are uploaded <br />
<br />
<br />
To run use following commands:<br />
1. for seeing yolov3-tiny output- $./darknet detector demo cfg/coco.data cfg/yolov3-tiny.cfg yolov3-tiny.weights Driving-Chinatown-SF.mp4<br />
2. for seeing yolov3 output-$./darknet detector demo cfg/coco.data cfg/yolov3.cfg yolov3.weights Driving-Chinatown-SF.mp4 <br />
3. for running saving output.mp4/.mov- $python3 yolo.py -w=yolov3-tiny.weights -cfg=cfg/yolov3-tiny.cfg -v=Market\ street.mp4  -l=data/coco.names<br />
