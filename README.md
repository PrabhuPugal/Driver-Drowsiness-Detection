# Driver Drowsiness Detection

## Description
**Driver Drowsiness Detection** is a machine learning project designed to detect signs of driver drowsiness using Convolutional Neural Networks (CNNs). The system analyzes video input from a camera to monitor the driver's eye movements and other facial features. If the system detects signs of drowsiness, such as closed eyes for a prolonged period, it triggers an alarm to alert the driver. This project aims to enhance road safety by preventing accidents caused by drowsy driving.

## Features
- **Real-Time Detection**: The system processes video input in real-time to monitor the driver's state of alertness.
- **CNN Model**: Utilizes a Convolutional Neural Network to accurately detect eye closure and other signs of drowsiness.
- **Alarm System**: An audible alarm (`rooster.mp3`) is triggered if drowsiness is detected, helping to wake up the driver.
- **Image Dataset**: The project uses a dataset of images that are preprocessed and categorized into different classes (e.g., eyes open, eyes closed) for training the CNN model.

## Technology Stack
The project is built using the following technologies:

- **Python**: The primary programming language used for data processing, model training, and detection.
- **OpenCV**: A computer vision library used for video processing and facial feature extraction.
- **TensorFlow/Keras**: A deep learning framework used to build and train the Convolutional Neural Network.
- **Jupyter Notebook**: Used for developing and testing the machine learning model (`Driver Drowsiness Detection using CNN.ipynb`).

## Dataset
The project uses a custom image dataset consisting of:

- **F_CLOSED**: Contains images of faces with closed eyes.
- **F_OPENED**: Contains images of faces with open eyes.
- **CROPPED**: Contains cropped images focusing on the eyes to improve the model's detection accuracy.

The dataset is used to train the CNN model to distinguish between open and closed eyes, which is crucial for detecting drowsiness.

## How It Works
1. **Video Input**: The system captures video input from a camera focused on the driver's face.
2. **Feature Extraction**: Using OpenCV, the system detects the driver's face and extracts the region of interest (eyes).
3. **CNN Model**: The extracted features are passed through the trained CNN model to determine if the driver's eyes are open or closed.
4. **Drowsiness Detection**: If the eyes are detected as closed for a certain duration, the system concludes that the driver is drowsy.
5. **Alarm Trigger**: An alarm sound (`rooster.mp3`) is played to alert the driver and prevent potential accidents.

## Model Training
1. Architecture: The CNN model is designed with multiple convolutional layers followed by pooling layers, dense layers, and a final softmax output layer.
2. Training: The model is trained using the preprocessed image dataset, with separate classes for open and closed eyes.
3. Evaluation: The model is evaluated on a validation set to ensure its accuracy in detecting drowsiness.

## Future Enhancements
1. Integration with Vehicle Systems: Implement the system in real vehicles, integrating it with the car's alert mechanisms.
2. Improved Accuracy: Enhance the model by using a larger and more diverse dataset, and experimenting with different deep learning architectures.
3. Additional Features: Incorporate additional drowsiness indicators such as yawning or head nodding to improve detection reliability.

## Contributing
Contributions are welcome! To contribute to the Driver Drowsiness Detection project, please follow these steps:
1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and test thoroughly.
4. Submit a pull request with a clear description of the changes.
5. Please ensure that your code adheres to the project's coding standards and includes appropriate documentation.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.

## Contact
For questions or feedback, please reach out to me at prabhupugal01@gmail.com.
