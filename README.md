# Garbage Classification Project Using VGG16 and MobileNetV2

## Project Overview
This project utilizes deep learning models, specifically VGG16 and MobileNetV2, to classify household garbage into multiple categories. The objective is to enhance the efficiency of recycling processes by accurately sorting garbage into its respective classes.

## Models Used
- **VGG16**: Known for its depth and high accuracy in image classification tasks but requires substantial computational resources.
- **MobileNetV2**: Designed for efficiency, performs well in environments with limited computational capacity, achieving high accuracy with less resource consumption.

## Dataset
The dataset, sourced from Kaggle, comprises 15,150 images across eight distinct classes: brown-glass, cardboard, clothes, green-glass, metal, paper, plastic, and white-glass. These categories were specifically chosen to cover a broad range of commonly recycled materials.

## Setup and Configuration
### Prerequisites
- Python 3.8 or above
- TensorFlow 2.x
- OpenCV
- Matplotlib

### Installation
1. Clone the repository:
   ```
   git clone https://github.com/GitUsmanBaig/EcoClassifier
   ```
2. Install the required packages:
   ```
   pip install tensorflow matplotlib opencv-python-headless
   ```

## Usage
To train the models and evaluate their performance:
1. Navigate to the project directory.
2. Run the training script:
   ```
   python MobileNetV2.py
   python vgg16.py
   ```

## Training Process
- **Data Preparation**: Utilizes `ImageDataGenerator` for image resizing, normalization, and augmentation.
- **Model Training**:
  - VGG16 trained for 2 epochs due to computational limits, achieving ~80% accuracy.
  - MobileNetV2 extended to 13 epochs, achieving ~92% accuracy.

## Challenges
- **Computational Resource Constraints**: Limited by the capabilities of standard laptops, particularly with VGG16.
- **Dependency on Stable Internet**: Required for training in cloud environments like Google Colab.
- **Duration of Model Training**: Extensive training periods necessary for achieving high accuracy.

## Conclusion
The project highlights the effectiveness of MobileNetV2 for tasks requiring high efficiency with constrained resources, whereas VGG16, though highly accurate, is best suited for scenarios with substantial computational capabilities.
