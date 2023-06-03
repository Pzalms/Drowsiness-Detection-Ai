# Drowsiness-Detection-Ai
# Drowsiness Detection AI using YOLOv5 in Python Notebook

This repository contains code for a drowsiness detection AI system using YOLOv5 in a Python notebook. The system utilizes the YOLOv5 object detection algorithm to detect faces and eyes in real-time video streams, and then employs a drowsiness detection algorithm to determine if the person is drowsy or not.

## Prerequisites
- Python 3.6 or above
- PyTorch
- OpenCV
- numpy

## Installation

1. Clone the repository:

```bash
git clone https://github.com/pzalms/drowsiness-detection-ai.git
```

2. Install the required dependencies:


## Usage

1. Launch Jupyter Notebook:

2. Open the  notebook in the Jupyter Notebook interface.

3. Follow the instructions in the notebook to run the drowsiness detection AI system.

## Model Training (Optional)

If you want to train your own drowsiness detection model, you can follow these steps:

1. Prepare your dataset of drowsy and non-drowsy images.

2. Split your dataset into training and validation sets.

3. Convert your dataset to the YOLO format. You can use the `labelImg` tool or any other annotation tool to annotate your images and generate the necessary labels.

4. Place the training and validation images along with the corresponding YOLO labels in the `data` directory.

5. Modify the training configuration in the `train.py` file if needed.

6. Run the training script:

```bash
python train.py --data data/dataset.yaml --cfg models/yolov5s.yaml --weights '' --batch-size 16 --epochs 100
```

7. Once the training is complete, you will find the trained model weights in the `runs/train/expX/weights` directory.

## License

This project is licensed under the [MIT License](LICENSE).

## Acknowledgments

- This project is based on the YOLOv5 implementation by Ultralytics. You can find their repository [here](https://github.com/ultralytics/yolov5).

## References

- [YOLOv5 repository](https://github.com/ultralytics/yolov5)
- [YOLO: Real-Time Object Detection](https://pjreddie.com/darknet/yolo/)
- [Drowsiness Detection with OpenCV](https://www.pyimagesearch.com/2017/05/08/drowsiness-detection-opencv/)
