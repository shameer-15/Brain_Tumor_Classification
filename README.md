



# Brain Tumor Classification

## Overview

This project aims to classify brain tumors using deep learning techniques. It uses Convolutional Neural Networks (CNNs) to classify MRI scans into different categories: glioma, meningioma, and pituitary tumor.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Model Architecture](#model-architecture)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Installation

To set up the project, follow these steps:

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/shameer-15/Brain_Tumor_Classification.git
   cd Brain_Tumor_Classification
   ```

2. **Create a Virtual Environment:**

   ```bash
   python -m venv venv
   ```

3. **Activate the Virtual Environment:**

   - **Windows:**

     ```bash
     venv\Scripts\activate
     ```

   - **macOS/Linux:**

     ```bash
     source venv/bin/activate
     ```

4. **Install Dependencies:**

   ```bash
   pip install -r requirements.txt
   ```

## Usage

1. **Prepare the Dataset:**
   Place your MRI scans in the `data` directory. Ensure that the data is organized into subdirectories based on the tumor type.

2. **Train the Model:**

   Run the training script:

   ```bash
   python train.py
   ```

3. **Evaluate the Model:**

   Run the evaluation script:

   ```bash
   python evaluate.py
   ```

4. **Make Predictions:**

   Use the prediction script:

   ```bash
   python predict.py --image_path <path_to_image>
   ```

## Dataset

The dataset used in this project consists of MRI scans of brain tumors. It is divided into the following classes:

- Glioma
- Meningioma
- Pituitary Tumor

Ensure that your dataset follows this structure:

```
data/
  glioma/
    image1.jpg
    image2.jpg
    ...
  meningioma/
    image1.jpg
    image2.jpg
    ...
  pituitary_tumor/
    image1.jpg
    image2.jpg
    ...
```

## Model Architecture

This project utilizes a Convolutional Neural Network (CNN) with the following architecture:

- **Input Layer**: Accepts images of size 224x224x3
- **Convolutional Layers**: Several convolutional layers with ReLU activation
- **Pooling Layers**: MaxPooling layers to reduce dimensionality
- **Fully Connected Layers**: Dense layers for classification
- **Output Layer**: Softmax activation to classify into three categories

## Results

The model's performance can be evaluated using accuracy, precision, recall, and F1 score. Results are saved in `results/` directory after evaluation.

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request with your improvements or bug fixes.

1. **Fork the Repository**
2. **Create a New Branch:**

   ```bash
   git checkout -b feature-branch
   ```

3. **Commit Your Changes:**

   ```bash
   git add .
   git commit -m "Add new feature"
   ```

4. **Push to the Branch:**

   ```bash
   git push origin feature-branch
   ```

5. **Submit a Pull Request**

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.

---

Feel free to modify this README to fit the specific details of your project, including any additional setup steps, custom scripts, or particular model details. Let me know if you need any more help!
