Sure! Here's the entire `README.md` content in **one single code block**, ready to paste:

````markdown
# 🍃 Tea Leaf Disease Detection using YOLOv8

This project leverages **YOLOv8** (You Only Look Once v8), a state-of-the-art real-time object detection model, to detect and classify diseases in tea leaves from images. The goal is to assist farmers and researchers in early identification of tea plant diseases to ensure better yield and plant health.

## 🚀 Features

- Trained YOLOv8 model for tea leaf disease detection
- Custom dataset preparation and annotation
- Real-time inference on images and videos
- Easy-to-use interface for testing predictions
- Model evaluation metrics and performance visualization

## 📁 Project Structure

```
tea-leaf-disease-yolov8/
├── dataset/
│   ├── images/
│   ├── labels/
├── runs/
├── weights/
│   └── best.pt
├── notebooks/
│   └── training_pipeline.ipynb
├── predict.py
├── train.py
├── requirements.txt
└── README.md
```

## 🧠 Tea Leaf Diseases Covered

- Gray Blight
- Red Rust
- Tea Mosquito Bug
- Healthy Leaf

## 🔧 Requirements

Install the necessary dependencies with:

```bash
pip install -r requirements.txt
```

## 🏋️‍♂️ Training

To train the model on your dataset:

```bash
yolo task=detect mode=train model=yolov8n.pt data=dataset.yaml epochs=100 imgsz=640
```

## 📈 Evaluation

Evaluate the model performance:

```bash
yolo task=detect mode=val model=weights/best.pt data=dataset.yaml
```

## 🔍 Inference

Run detection on an image:

```bash
yolo task=detect mode=predict model=weights/best.pt source=path/to/image.jpg
```

Or on a video/webcam:

```bash
yolo task=detect mode=predict model=weights/best.pt source=0
```

## 📊 Results

- mAP (mean Average Precision): XX%
- Precision: XX%
- Recall: XX%

> *(Replace `XX` with your actual evaluation results.)*

## 📸 Sample Predictions

Add some images here (optional):

```
Before:
[image of input]

After:
[image with detection boxes]
```

## 📝 Dataset

The dataset was custom-labeled using [Roboflow](https://roboflow.com/) / LabelImg. It contains annotated images for each class.

## 🙌 Acknowledgements

- [Ultralytics YOLOv8](https://github.com/ultralytics/ultralytics)
- [Roboflow](https://roboflow.com/)
- All contributors and open-source community

## 📄 License

This project is licensed under the [MIT License](LICENSE).
````

Let me know if you'd like a version that includes badges, Streamlit UI, or Colab links.
# Tea_leaf_disease_YoloV8
