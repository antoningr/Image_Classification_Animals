📄 GitHub Documentation

# 🧠 Vision Transformer (ViT) Image Classifier

This project demonstrates how to use a pre-trained Vision Transformer (ViT) model from Hugging Face Transformers to classify animal images using a dataset downloaded from Kaggle via `kagglehub`.


## 📂 Dataset

We use the [Animal Image Dataset (90 categories)](https://www.kaggle.com/datasets/iamsouravbanerjee/animal-image-dataset-90-different-animals), which contains labeled images of 90 different animals. The dataset is automatically downloaded using `kagglehub`.


## 🚀 What This Notebook Does

- Downloads and loads the animal image dataset
- Uses the `google/vit-base-patch16-224` model from Hugging Face
- Classifies up to 10 images using ImageNet labels
- Displays images with the predicted class


## 🛠️ Requirements

Install the necessary libraries:

```bash
pip install transformers torch Pillow kagglehu
```

## 📘 Language
python

# Download the dataset using kagglehub
```
import kagglehub

# Download latest version
path = kagglehub.dataset_download("iamsouravbanerjee/animal-image-dataset-90-different-animals")

print("Path to dataset files:", path)
```

## 🧠 Model Used
google/vit-base-patch16-224
Pretrained Vision Transformer model, fine-tuned on ImageNet-1k.

## 📄 License
Apache 2.0 – based on ViT paper and Hugging Face models.

## 🙌 Credits
Hugging Face
KaggleHub