objRecognizer

Requirements:
- tensorflow >= 2.2.*
- keras > 2.3.*

**For YOLO model**
1. Download these files
wget https://storage.googleapis.com/kent-test/ai_school/yolo/utils.py
wget https://storage.googleapis.com/kent-test/ai_school/yolo/preprocessing.py

2. Download the pre-trained weights of YOLO
!wget https://storage.googleapis.com/kent-test/ai_school/weights_coco.h5
save weights_coco.h5 in model_data/

3. Run the .ipynb file in Google colab

(The input image: test_data/test_img.jpg, the output image: results/test_img_bbox.jpg)
(The input video: test_data/street.mp4, the output video: results/street_bbox.mp4)




**For YOLO v3 model**
1. Download yolov3.weights
!wget -P model_data https://pjreddie.com/media/files/yolov3.weights
and save yolov3.weights in model_data/

2. Run: yolov3_model_training.py
save the mode in model_data/yolo3_saved_model.h5

3. Run yolov3_model_predict_image.py to recognize objects in a image
test image: test_data/test_img.jpg
output: results/img_bbox_yolo_v3.jpg

4. Run yolov3_model_predict_video.py to recognize objects in a video
test video: test_data/street.mp4
output: test_data/street_bbox_yolo_v3.mp4
