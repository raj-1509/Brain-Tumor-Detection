## Brain Tumor Detection using-U-Net with Attention for Multi-Class Image Classification

This project implements a U-Net architecture enhanced with Attention Gates for multi-class image classification using TensorFlow/Keras. The trained model is deployed using FastAPI and served over the web via `ngrok` on Google Colab.

---

## 🧠 Model Overview

- **Architecture**: U-Net with Attention Blocks
- **Input Shape**: 224 x 224 x 3
- **Output**: Softmax over 4 classes
- **Key Features**:
  - Attention Blocks between encoder and decoder
  - Batch Normalization and Dropout for regularization
  - Fully Connected classifier at the bottleneck

---

## 🚀 Deployment via FastAPI on Google Colab

### ✅ Requirements

Run the following to install dependencies:
```bash
!pip install tensorflow fastapi uvicorn pyngrok nest_asyncio
## 🧪 Models Explored

### 1. **ConvAttention**
- Combines convolutional layers with spatial and channel-wise attention.
- Enhances focus on tumor regions by prioritizing spatial proximity of features.
- Accuracy achieved: **93.06%**

### 2. **Standard U-Net**
- Encoder-decoder structure with skip connections.
- Strong baseline model for biomedical image segmentation.
- Accuracy achieved: **91.53%**

### 3. **Attention-Based U-Net (Proposed)**
- U-Net integrated with self-attention blocks between encoder-decoder.
- Captures long-range dependencies and better spatial context.
- Accuracy achieved: **95.50%**

---

## 📊 Dataset

- **Source**: Public MRI dataset containing four categories:
  - Glioma
  - Meningioma
  - Pituitary
  - No Tumor
- **Preprocessing**:
  - Resizing to `224x224`
  - Normalization
  - Data augmentation: rotation, flipping, zooming

---



