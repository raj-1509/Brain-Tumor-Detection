🧠 Attention-Based U-Net for Enhanced Brain Tumor Classification
This project explores the effectiveness of integrating attention mechanisms into the U-Net architecture for improved brain tumor classification using MRI data. It compares multiple deep learning models including ConvAttention, standard U-Net, and the proposed Attention-Based U-Net.

📁 Project Structure
Brain-Tumor-Classification/
│
├── Brain_Tumor_Detection.ipynb   # Jupyter notebook for model implementation
├── dataset/                      # MRI images categorized into 4 tumor classes
│   ├── glioma/
│   ├── meningioma/
│   ├── pituitary/
│   └── no_tumor/
│
├── models/                       # Python scripts for model definitions (optional)
├── results/                      # Plots: confusion matrices, accuracy/loss graphs
├── saved_models/                # Trained model weights
├── README.md                    # Project documentation
└── requirements.txt             # Dependencies


🧪 Models Explored
1. ConvAttention
Combines convolutional layers with spatial and channel-wise attention.
Enhances focus on tumor regions by prioritizing spatial proximity of features.
Accuracy achieved: 93.06%

2. Standard U-Net
Encoder-decoder structure with skip connections.
Strong baseline model for biomedical image segmentation.
Accuracy achieved: 91.53%

3. Attention-Based U-Net (Proposed)
U-Net integrated with self-attention blocks between encoder-decoder.
Captures long-range dependencies and better spatial context.
Accuracy achieved: 95.50%

📊 Dataset
Source: Public MRI dataset containing four categories:
Glioma
Meningioma
Pituitary
No Tumor

Preprocessing:
Resizing to 224x224
Normalization
Data augmentation: rotation, flipping, zooming



📌 Key Contributions
Introduced attention-enhanced U-Net architecture for improved feature focus.
Demonstrated higher segmentation accuracy than existing CNN/U-Net models.
Validated performance via comprehensive metrics and visualizations.
