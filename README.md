# Face mask detection on Yolo V7
 In this is work we retrained YoloV7 model on face mask detection task

Original model was provided by https://github.com/WongKinYiu/yolov7.

Model was retrained on [this](https://www.kaggle.com/datasets/andrewmvd/face-mask-detection?resource=download) dataset.

Here you can find weights to the model.

To inferense model use:
``` shell
!python detect.py --weights runs/train/exp4/weights/best.pt --conf 0.1 --source <path_to_your_folder_or_jpeg_file>
```
