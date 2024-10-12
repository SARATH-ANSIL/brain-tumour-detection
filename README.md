# Brain Tumor Detection

This project implements a brain tumor detection system using Convolutional Neural Networks (CNN) on MRI images. The model classifies brain MRI images into two categories: tumorous and non-tumorous.

## Features
- **Image Augmentation:** Utilizes techniques to artificially increase the size of the training dataset.
- **Custom Model Architecture:** Implements a CNN model to classify MRI images based on the presence of a tumor.
- **Data Visualization:** Provides visualization of training metrics and sample images.

## Prerequisites
Make sure you have the following installed:
- Python 3.x
- The following Python libraries must be installed:
  - `numpy`
  - `pandas`
  - `tensorflow`
  - `keras`
  - `opencv-python`
  - `matplotlib`
  - `imutils`
  
You can install the required libraries using pip:
```bash
pip install numpy pandas tensorflow keras opencv-python matplotlib imutils
```
## Project Structure
```bash
.
├── brain-tumour-detection.ipynb  # Main Jupyter Notebook for training and testing the model
├── output/                        # Directory for storing output images
│   └── kaggle/
│       └── working/
│           └── augmented-images/  # Directory for storing augmented images
│               ├── yes/           # Augmented images with tumor
│               └── no/            # Augmented images without tumor
└── README.md                      # Project README file
```
## How It Works
- **Installing Dependencies**: The project uses libraries for image processing and deep learning.

- **Loading Images**: MRI images are loaded from a specified directory, which contains images categorized into 'yes' (tumorous) and 'no' (non-tumorous).

- **Image Augmentation**: The dataset is augmented to generate more samples for training, improving the model's robustness.

- **Cropping**: The model applies a cropping technique to focus on the relevant part of the images containing tumors.

- **Data Preprocessing**: The images are resized, normalized, and prepared for training.

- **Model Building**: A CNN architecture is built using Keras, consisting of convolutional, pooling, and dense layers.

- **Model Training**: The model is trained using the training dataset and validated using a separate validation dataset.

- **Metrics Visualization**: The training and validation metrics are plotted to analyze the model's performance.

## Running the Project
Clone the repository and navigate to the project directory.

Open the Jupyter Notebook:
`jupyter notebook brain-tumour-detection.ipynb`

Follow the instructions in the notebook to install dependencies, load data, and train the model.

Analyze the training metrics and visualize the results.

## Example Output
After running the training and testing scripts, the results will include visualizations of the training and validation loss and accuracy over epochs.

## Contributing
Contributions, issues, and feature requests are welcome! Feel free to check the issues page for new ideas.

## License
This project is licensed under the MIT License.

## Acknowledgments
TensorFlow and Keras for deep learning functionalities.
OpenCV for image processing capabilities.
Matplotlib for plotting and visualizing data.
