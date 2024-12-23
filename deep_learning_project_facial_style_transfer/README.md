
# **DeepCanvas: Celebrity Image Classification and Style Transfer**

This project combines **image classification** and **neural style transfer** techniques to explore advanced computer vision tasks. The work involves recognizing and categorizing celebrity faces using deep learning and transforming these images into artistic styles. The project is divided into two main tasks: **Facial Recognition & Classification** and **Neural Style Transfer (NST)**.

---

## **Project Structure**
### **1. Classification**
- **[Classification_CNN.ipynb](Classification_CNN.ipynb)**: A Convolutional Neural Network (CNN) trained on the LFW dataset to classify celebrity images. Achieved an accuracy of **90.48%**.
- **[Classification_YOLO.ipynb](Classification_YOLO.ipynb)**: Leveraged the YOLOv5s model for real-time face detection and recognition with an average confidence score of **0.55**.

### **2. Style Transfer**
- **[StyleTransfer_Classical.ipynb](StyleTransfer_Classical.ipynb)**: Implements Classical Neural Style Transfer (NST) using the pre-trained VGG16 model for high-quality artistic transformations.
- **[StyleTransfer_AdaIN.ipynb](StyleTransfer_AdaIN.ipynb)**: Uses Adaptive Instance Normalization (AdaIN) for real-time style transfer, offering speed and simplicity.

---

## **Dataset**
- **LFW People Dataset**: Contains **13,233 images** of **1,680 individuals**, used for classification. 
  - Images are labeled and resized for training.
  - [Source](https://www.kaggle.com/datasets/atulanandjha/lfwpeople/)

- **Artworks Dataset**: Used for style images in the NST task.
  - [Source](https://www.kaggle.com/datasets/ikarus777/best-artworks-of-all-time)

---

## **Tasks and Models**

### **Task 1: Facial Recognition and Classification**
- **Objective**: Identify and classify celebrity faces.
- **Methods**:
  1. **CNN**: Focused on feature extraction and classification.
  2. **YOLOv5s**: Optimized for speed and accuracy in object detection.

### **Task 2: Neural Style Transfer**
- **Objective**: Transform celebrity images into artistic styles.
- **Methods**:
  1. **Classical NST**: Utilizes VGG16 to compute content and style losses.
  2. **AdaIN**: Adapts feature maps for style transfer in real-time.

---

## **Results**
- **Classification**:
  - CNN achieved **90.48% accuracy**.
  - YOLOv5s demonstrated a balance between speed and accuracy with an **average confidence score of 0.55**.
- **Style Transfer**:
  - **Classical NST**: Produced high-quality results with fine details.
  - **AdaIN**: Delivered faster and simpler results suitable for real-time applications.

---

## **How to Run**
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/DeepCanvas.git
   ```
2. Navigate to the project folder:
   ```bash
   cd DeepCanvas
   ```
3. Open the desired `.ipynb` file in Jupyter Notebook or Google Colab:
   - **Classification**: 
     - [Classification_CNN.ipynb](Classification_CNN.ipynb)
     - [Classification_YOLO.ipynb](Classification_YOLO.ipynb)
   - **Style Transfer**:
     - [StyleTransfer_Classical.ipynb](StyleTransfer_Classical.ipynb)
     - [StyleTransfer_AdaIN.ipynb](StyleTransfer_AdaIN.ipynb)

---

## **References**
- [LFW People Dataset](https://www.kaggle.com/datasets/atulanandjha/lfwpeople/)
- [YOLOv5s](https://github.com/ultralytics/yolov5/releases)
- [AdaIN Style Transfer](https://keras.io/examples/generative/adain/)
- [Artworks Dataset](https://www.kaggle.com/datasets/ikarus777/best-artworks-of-all-time)

---
