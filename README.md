# Plant Detection and Face Recognition

This repository contains two folders: "Plant Detection" and "Face Recognition." In these folders, I have built their respective models using transfer learning from YOLOv5x.

## Plant Detection

For the plant detection task, I trained a YOLOv5s (small) model on the PlantDoc dataset sourced from Roboflow. The dataset contains 2,569 images across 13 plant species and 30 classes, totaling 8,851 labels. The model was trained to accurately predict various plant images.

## Face Recognition

For the face recognition task, I collected images of two people - my friend and myself. I labeled these images using Makesense.ai and trained a face recognition model using YOLOv5x.

# How to Run:

1. Clone the YOLOv5 repository into the project directory using the following command:
    git clone https://github.com/ultralytics/yolov5

2. Install the required dependencies by running:
    pip install -r yolov5/requirements.txt


3. To test the model predictions, use the following command:
    python yolov5/detect.py --weights xx --source yy

Replace `xx` with either `yolov5x/yolov5x.pt` for YOLOv5x or `plant_detection/results/best_model.pt` for plant detection mode, or `face_recognition/results/best_model.pt` for the face recognition mode.
Replace `yy` with the path to the image or video you want to run the model on. To use the camera input, set `--source 0`.

The results will be saved in the `yolov5/runs` directory.

Please feel free to explore the code for both use cases. If you have any questions or encounter any issues, do not hesitate to reach out. Happy coding!
