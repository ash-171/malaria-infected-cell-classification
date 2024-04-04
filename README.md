# Malaria-Infected Cell Classification Dashboard

## Introduction
This project aims to build an explainable deep learning model to classify malaria-infected cells using the Cell Images for Detecting Malaria dataset. The model is deployed in a simple dashboard to provide an interactive interface for users to classify images of cells as either infected or uninfected.

## Dataset
The dataset contains a total of 27,560 images, with 13,780 parasitized (infected) images and 13,780 uninfected images. The dataset was sourced from [Kaggle](https://www.kaggle.com/datasets/iarunava/cell-images-for-detecting-malaria).

## Model Architecture
For this classification task, we used a Convolutional Neural Network (CNN) architecture. The model consists of multiple convolutional layers followed by max-pooling layers for feature extraction, followed by fully connected layers for classification. We chose this architecture due to its effectiveness in learning spatial hierarchies of features in image data.

## File Structure
The file structure for this project is as follows:
```
├── models/
│   ├── artifacts/
│   │   ├── model.h5
│   ├── data/
│   │   ├── Parasitized/
│   │   └── Uninfected/
│   └── src/
│       └── model.ipynb
├── Dockerfile
├── packages.txt
├── demo.mp4
├── report.pdf
├── requirements.txt
├── LICENSE
└── README.md
```

## Model Deployment
The trained model is deployed in a simple dashboard using Streamlit. Users can upload an image of a cell, and the dashboard will classify it as infected or uninfected. The hotspots influencing the prediction are overlaid on the image to provide insights into the model's decision-making process.

## Instructions
To reproduce this project or run the dashboard locally, follow these steps:

1. Clone the repository:
    ```bash
    git clone https://github.com/ash-171/malaria-infected-cell-classification.git
    cd malaria-infected-cell-classification
    ```

2. Install the required dependencies by running:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the Streamlit app:
    ```bash
    streamlit run src/app.py
    ```

4. Upload an image of a cell to the dashboard and observe the classification results along with the overlaid hotspots.

## Credits
- Dataset: [Cell Images for Detecting Malaria](https://www.kaggle.com/datasets/iarunava/cell-images-for-detecting-malaria)
- Assignment by IQGateway

For any further questions or assistance, please reach out to mailaswathits@gmail.com.
