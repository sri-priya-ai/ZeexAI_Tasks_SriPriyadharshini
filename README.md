#  EcoVisionNet — Satellite Image Classification

##  Overview
EcoVisionNet is a deep learning project that classifies satellite images into different land-cover types such as vegetation, water, and urban areas.  
It uses the **EuroSAT dataset** (Sentinel-2 RGB images) and a fine-tuned **ResNet-18** model. Grad-CAM visualizations are used to explain model predictions.
Dataset Details

Dataset: EuroSAT (RGB version)

Source: Sentinel-2 satellite imagery

Classes: Forest, River, Residential, Industrial, Highway, Pasture, etc.

Image size: 64×64 RGB

Sri Priyadharshini T
B.E. Computer Science and Engineering
Results

Model Used: ResNet-18 (fine-tuned)

Accuracy: ~90% after several epochs

Evaluation Metrics: Accuracy, Loss curve, and Grad-CAM visualizations

---

##  Setup Instructions
If you are running this project in **Google Colab**, run the following command first to install all dependencies:

```bash
!pip install tensorflow gradio matplotlib numpy pandas

