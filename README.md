# EcoVisionNet

EcoVisionNet is a deep learning project built to classify land cover types from satellite images using the **EuroSAT (Sentinel-2 RGB)** dataset. It combines a **Custom CNN** with **ResNet-18 (transfer learning)** and includes **Grad-CAM visualization** for explainable AI insights. The project is developed and run entirely in **Google Colab**.

---

##  Project Overview

EcoVisionNet identifies different land cover types such as **Forest, River, Residential, Industrial, Highway, and Pasture** using deep learning models trained on satellite imagery. The model is explainable through Grad-CAM visualizations that highlight regions of the image most responsible for predictions.

---

## What I Did in Colab

### 1. Project Setup
- Created a new Google Colab notebook named **EcoVisionNet.ipynb**.  
- Installed required libraries
- - Imported all dependencies (TensorFlow, Keras, Matplotlib, Pandas, NumPy, etc.) and verified the runtime environment.

### 2. Dataset
- Used the **EuroSAT (Sentinel-2 RGB)** public dataset for satellite-based land cover classification.  
- Loaded the dataset with image size **64×64 RGB** and inspected the data distribution.  
- Prepared the dataset for training and testing splits.

### 3. Preprocessing
- Normalized all image pixel values for stable model training.  
- Created training and testing data batches.  
- Verified dataset shape and balance before training.

### 4. Model Development
- Built a **hybrid model combining Custom CNN layers and pretrained ResNet-18 (transfer learning)**.  
- Added additional Dense, Dropout, and Activation layers for EuroSAT classification.  
- Fine-tuned the pretrained model on the specific satellite dataset.

### 5. Model Training
- Used **Adam optimizer** and **categorical cross-entropy loss**.  
- Tracked model performance through **accuracy and loss graphs** during training.  
- Evaluated the final model on test data to obtain the overall accuracy score.

### 6. Explainable AI (Grad-CAM)
- Implemented **Grad-CAM** visualization to interpret model decisions.  
- Generated heatmaps for several test images to show which image regions influenced predictions most.  
- Displayed side-by-side results of input images and activation maps.

### 7. Gradio User Interface
- Integrated a **Gradio app** directly in the Colab notebook:
- Upload a satellite image.
- Get the predicted class.
- View Grad-CAM heatmap highlighting the decision regions.

### 8. Results & Outputs
- Achieved strong classification accuracy on test data.  
- Produced clear Grad-CAM heatmaps validating predictive interpretability.  
- Verified the model’s real-time functionality using the Gradio interface.

---

##  How to Reproduce in Google Colab

To view or re-run the results, follow these simple steps:

1. **Open the Notebook**
 - Upload or open `EcoVisionNet.ipynb` in Google Colab.

2. **Run All Cells**
 - Click **Runtime → Run All** to execute all code blocks sequentially.
 - The notebook will automatically:
   - Download the EuroSAT dataset.
   - Preprocess and split data.
   - Train the hybrid CNN + ResNet model.
   - Display accuracy/loss graphs.
   - Generate Grad-CAM visualizations.

3. **Interact with Gradio UI**
 - At the end of the notebook, the Gradio app will appear.
 - Upload a satellite image to see:
   - Predicted land cover class.
   - Grad-CAM heatmap overlay for explainability.

4. **Check Outputs Folder **
 - All generated plots and Grad-CAM results will be displayed within the Colab notebook.
 - Additional screenshots and results can be viewed in the **screenshots/** folder included in the repository.

---




