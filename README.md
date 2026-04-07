# 🚀 U-Net Nuclei Segmentation 
This project implements a U-Net architecture for binary semantic segmentation of cell nuclei using BBBC039 dataset. This model achieves a dice score of **0.8600** on the test set. 

## 💻 Environment Details
+ **Platform:** Google Colab
+ **Python Version:** 3.10
+ **Framework:** PyTorch
+ **Hardware Used:** NVIDIA T4 GPU
+ **Random Seed:** 42 (or Default/None if not explicitly set)

## 🛠️ Dependencies
To install the required libraries, run:
```console
```bash
pip install -r requirements.txt
```
## 📂 Project Structure
```
.
├── requirement.txt
├── training.ipynb
├── best_model_150.pth
└── Dataset
    └── data/
        └── binary_masks/
        └── images/
        └── masks/
        └── metadata/
```
## 🔹 Prepration
Make sure to have dataset folders in "My Drive" on Google Drive
Drop the "Dataset" folder to My Drive
```
└── Dataset
    └── data/
        └── binary_masks/
        └── images/
        └── masks/
        └── metadata/
```
## 🚀 Running the Project
1. Open the Notebook (training) in Google Colab
2. Setup Data: ensure the BBBC039 dataset is available
3. Initialize: Run the cells in Section 1, 3, 4 to load the libraries, mount drive, dataset class and U-Net model
4. Load Weight: To skip training and verify the result immediatly, ensure best_model_150.pth is in directory and run the Evaluation cell at the bottom of the notebook
5. Train (Optional): To retrain from scratch, run all cells from the top. Note that full training (150 epochs) takes around 30min on T4 GPU
