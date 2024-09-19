# Research Brain Tumor Radiogenomic Classification

## Overview
This project focuses on classifying glioblastoma, a type of brain tumor, using multi-parametric MRI (mpMRI) scans to predict the MGMT promoter methylation status—a key factor in determining treatment response. We employ deep learning models, including the MedViT (Vision Transformer) and other state-of-the-art architectures, to achieve accurate and non-invasive classification.

## Project Structure
- **Dataset**: Includes 672 MRI scans provided by the RSNA-MICCAI Brain Tumor Radiogenomic Classification Challenge. The dataset is split into training, validation, and testing sets, with scans in DICOM and PNG formats.
- **Models**:
  - **MedViT**: Integrates CNNs and Transformers for effective 3D MRI analysis.
  - **Transformer-based Model**: Combines EfficientNet-b0 for spatial features with a Transformer encoder for temporal modeling.
  - **EfficientNet-b0 with LSTM and Attention**: Processes different MRI modalities separately, followed by LSTM to capture temporal dependencies.

## Key Findings
- **MedViT** showed the highest validation accuracy (0.63), outperforming other models, highlighting its potential for reliable radiogenomic classification.
- Other models exhibited signs of overfitting, indicating the need for further tuning and additional regularization.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/QDuy0082/Research-Brain-Tumor-Radiogenomic-Classification.git
2. Install the required dependencies:
   ```bash
   pip install -r requirements.txt
## Usage
**Training:** To start model training, run the following command:
```bash
   python train_model.py
**Evaluation:** To evaluate the model on the validation or test set, use:
   ```bash
   python evaluate_model.py
## Results
The MedViT model outperformed other architectures in this project, achieving a validation accuracy of 0.63. However, further work is needed to refine the other models, which displayed some overfitting during training.

## Acknowledgments
This project was inspired by the RSNA-MICCAI Brain Tumor Radiogenomic Classification Challenge. Special thanks to Dr. Minh-Triet Tran for his invaluable guidance and to the entire team for their support.

## License
This project is licensed under the MIT License - see the LICENSE file for details.




