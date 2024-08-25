# Brain Tumor Detection Using YOLOv5

## Overview
This project demonstrates the use of YOLOv5 for brain tumor detection from medical images. The objective is to accurately detect and localize brain tumors within MRI scans by leveraging the YOLOv5 model, which is known for its speed and accuracy in object detection tasks.

## Dataset Description
The dataset used in this project consists of MRI images annotated with tumor locations. The annotations are originally in COCO format, which includes bounding box information and polygon points for segmentation.

### Dataset Structure
- **train/**: Training images and corresponding labels.
  - **images/**: MRI images used for training.
  - **labels/**: YOLO-formatted labels corresponding to the training images.
- **valid/**: Validation images and corresponding labels.
  - **images/**: MRI images used for validation.
  - **labels/**: YOLO-formatted labels corresponding to the validation images.
- **test/**: Test images and corresponding labels.
  - **images/**: MRI images used for testing.
  - **labels/**: YOLO-formatted labels corresponding to the test images.

## Model Architecture
The model used in this project is based on YOLOv5, which is a state-of-the-art object detection model. YOLOv5 offers a balance between detection accuracy and computational efficiency, making it suitable for real-time applications.

## Installation
To set up the environment and run the project, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/your-username/brain-tumor-detection.git
   cd brain-tumor-detection
   ```

2. **Install the required dependencies:**
   ```bash
   pip install -r requirements.txt
   ```

3. **Set up YOLOv5 in Google Colab:**
   Follow the instructions in the notebook to set up YOLOv5 for use in Google Colab.

## Usage Instructions
1. **Dataset Preparation:**
   - The dataset annotations are initially in COCO format. Use the provided parser script to convert the COCO annotations into YOLO format, where each image's bounding box and segmentation points are saved in `.txt` files.

2. **Organizing the Dataset:**
   - Ensure the images and their corresponding labels are organized in the `/train/images`, `/valid/images`, and `/test/images` directories as described.

3. **Training the Model:**
   - Use the provided notebook to train the YOLOv5 model on the prepared dataset. Adjust hyperparameters and configurations as necessary to achieve the best performance.

4. **Inference:**
   - After training, use the model to make predictions on new images. The `detect.py` script can be modified to save cropped images of detected tumors.

## Results
- The results of the model training, and validation and testing are detailed in the notebook. You can visualize the model's performance on the validation and test datasets using the provided scripts.

## Contributing
Contributions to this project are welcome! Please fork the repository and submit a pull request with your improvements or bug fixes.

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for more details.



