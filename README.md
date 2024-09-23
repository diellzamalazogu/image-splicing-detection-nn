# Image Splicing Detection using VGG-16, VGG-19, and ResNet-50

This project implements deep learning neural network models **VGG-16**, **VGG-19**, and **ResNet-50** on the **Columbia Image Splicing Detection dataset** to detect image forgery, specifically focusing on image splicing.

## Project Overview

In a world where digital manipulation is becoming increasingly common, this experiment seeks to address the challenge of detecting **image splicing** using state-of-the-art convolutional neural networks. By training and testing models on the Columbia dataset, this project aims to contribute to the detection of image forgery.

## Models Used
- **VGG-16**
- **VGG-19**
- **ResNet-50**

## Dataset

The dataset includes both training and testing sets, organized as follows:
- **Dataset.zip**:
  - `train/`: Contains spliced and original images for training.
    - `spliced/`
    - `original/`
  - `test/`: Contains spliced and original images for testing.
    - `spliced/`
    - `original/`

## Running the Code

Each model is implemented in a Jupyter notebook (`.ipynb`) and can be run on **Google Colab**. The code must be authorized to access **Google Drive** before executing the rest of the script.

To run the code, follow these steps:

1. **Set the path to the dataset**:
    ```python
    train_path = 'drive/ML/alpha/dataset/train'
    test_path = 'drive/ML/alpha/dataset/test'
    ```

2. **Model and Weights Saving**: The model and its weights will be saved to Google Drive. By default, they are saved to:
    ```python
    with open("drive/ML/CNNImageSplicingDetectorModel.json", "w") as json_file:
        json_file.write(model_json)

    # serialize weights to HDF5
    NEW_MODEL.save_weights("drive/ML/CNNImageSplicingDetectorModelWeights.h5")
    ```

## Files Included

- `VGG16_model.ipynb`
- `VGG19_model.ipynb`
- `ResNet50_model.ipynb`
- `Dataset.zip`

## Notes

- Ensure that Google Colab has access to Google Drive before running the code.
- You can modify the dataset paths in the code if needed.

