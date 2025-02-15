
# Anemia Detection Using Conjunctiva Images

This project aims to detect anemia using conjunctiva images. The approach involves preprocessing images, training a convolutional neural network (CNN) for feature extraction, and using a Random Forest classifier for the final classification.

## Table of Contents
- [Installation](#installation)
- [Project Structure](#project-structure)
- [Methodology](#methodology)
- [Results](#results)
- [Contributing](#contributing)


## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/HarshSaxena837/Detection_Of_Anemia_Using_Conjuctiva_Images.git
    cd Detection_Of_Anemia_Using_Conjuctiva_Images
    ```

2. Install the required packages:
    ```bash
    pip install -r requirements.txt
    ```

3. Ensure you have the dataset organized in the following structure:
    ```
    artifacts/
    ├── class_1/
    │   ├── img1.jpg
    │   ├── img2.jpg
    │   └── ...
    └── class_2/
        ├── img1.jpg
        ├── img2.jpg
        └── ...
    ```

## Project Structure

```
.
├── artifacts/
│   ├── class_1/
│   └── class_2/
├── requirements.txt
├── README.md
└── anemia_detection.py
```

## Methodology

1. **Data Collection and Preprocessing**:
    - Load conjunctiva images.
    - Resize images to 64x64 pixels.
    - Normalize pixel values.

2. **Feature Extraction**:
    - Use a CNN for feature extraction.
    - Layers include Conv2D, MaxPool2D, and GlobalAveragePooling2D.

3. **Classification**:
    - Extract features from the CNN.
    - Use Random Forest classifier for the final classification.

## Results

- The model achieved an accuracy of 95.78% on the test set.
- Confusion Matrix:
    ```
    [[251,  12],
     [  6, 158]]
    ```

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request or open an issue for any bugs, feature requests, or improvements.
