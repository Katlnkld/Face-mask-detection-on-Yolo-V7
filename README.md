# Face mask detection on Yolo V7
 In this is work we retrained YoloV7 model on face mask detection task

Original model was provided by https://github.com/WongKinYiu/yolov7.

Model was retrained on [this](https://www.kaggle.com/datasets/andrewmvd/face-mask-detection?resource=download) dataset.

[Here](runs/train/exp4/weights/best.pt) you can find weights to the model.
Training curves and confusiom matrix are in [this folder](runs/train/exp4/).

To inference model use:
``` shell
python detect.py --weights runs/train/exp4/weights/best.pt --conf 0.1 --source <path_to_your_folder_or_jpeg_file>
```
The result will be saved [here](runs/detect)

Inference of model on our team members you can see in [this folder](inference_on_our_team_members).
