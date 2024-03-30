# **Sign-Language-To-Text-and-Speech-Conversion 💬👋**

## **Abstract**

Sign language serves as a fundamental means of communication, especially for the deaf and dumb community. In this project, we present a real-time method utilizing neural networks for finger spelling based American Sign Language (ASL). We propose a convolutional neural network (CNN) approach to recognize hand gestures from camera images, aiming to bridge the communication gap for individuals using sign language.

**The Final Outcome Of Our Project:** 
- `hello_there.mp4`: [Video demonstrating the project]

## **Introduction**

American Sign Language (ASL) is pivotal for communication among the deaf and dumb community, who rely on non-verbal gestures due to communication barriers. Our project focuses on developing a model capable of recognizing fingerspelling-based hand gestures to form complete words. By training a CNN model, we aim to enable efficient communication through sign language.

## **Requirements**

With over 70 million deaf individuals worldwide, the significance of sign languages in facilitating communication and social inclusion cannot be overstated. Our project addresses the challenge of ensuring equal access to communication for people with disabilities by developing a user-friendly Human-Computer Interface (HCI) that understands American Sign Language.

## **Objective**

The primary objective is to create a computer software application and train a CNN model capable of interpreting images of hand gestures in American Sign Language. The system should convert recognized gestures into text and optionally into speech, enhancing communication accessibility.

## **Scope**

The system benefits both the deaf and dumb community and individuals unfamiliar with sign language. By interpreting sign language gestures, the system provides output in both text and speech formats, promoting inclusivity and bridging communication barriers.

## **Modules**

### **Data Acquisition**

- **Electromechanical Devices**: Utilize devices for precise hand configuration and position data. Although effective, this approach is costly and less user-friendly.
- **Vision-based Methods**: Utilize computer webcams to observe hand gestures, offering a cost-effective solution for natural interaction between humans and computers.

- 


### **Data Pre-processing and Feature Extraction**

- **Hand Detection**: Employ the MediaPipe library for image processing to detect hands from webcam images.
- **Image Processing**: Convert detected regions of interest (ROI) to grayscale images using OpenCV library. Apply Gaussian blur and thresholding techniques to enhance image quality.
- **Data Collection**: Gather images of different signs from various angles for sign letters A to Z.

![13](https://github.com/ShrutiNathavani/Sign-Language-To-Text-and-Speech/assets/77912009/174dc35f-e683-4bc8-9c89-1b6750d93850)
### **Gesture Classification**

- **Convolutional Neural Network (CNN)**: Utilize CNN for gesture classification. CNN is effective in solving computer vision problems and is equipped with layers like convolution, max-pooling, and fully connected layers for feature extraction and classification.

### **Text To Speech Translation**

- Translate recognized gestures into words using the `pyttsx3` library. This feature simulates real-life dialogue and enhances user experience.

## **Project Requirements**

### **Hardware Requirement:**
- Webcam

### **Software Requirement:**
- **Operating System**: Windows 8 and Above
- **IDE**: PyCharm
- **Programming Language**: Python 3.9
- **Python Libraries**: OpenCV, NumPy, Keras, MediaPipe, TensorFlow

## **System Diagrams**

### **System Flowchart**


![System Flowchart](https://github.com/ShrutiNathavani/Sign-Language-To-Text-and-Speech/assets/77912009/f6a9b8c3-a2b5-485b-977c-846bd689d5e9)


### **Use-case Diagram**


![Use-case diagram](https://github.com/ShrutiNathavani/Sign-Language-To-Text-and-Speech/assets/77912009/69e077ed-b12a-4a9a-9cb2-9d3d64b345f0)


### **DFD Diagram**


![DFD diagram](https://github.com/ShrutiNathavani/Sign-Language-To-Text-and-Speech/assets/77912009/85081d60-7dab-440f-b0f9-3f90b8a761d7)


### **Sequence Diagram**

![Sequence diagram](https://github.com/ShrutiNathavani/Sign-Language-To-Text-and-Speech/assets/77912009/f633d5c0-cbbf-43d4-a628-da79a46cfa88)


## **License**

This project is licensed under the [MIT License](LICENSE).

## **Acknowledgments**

- Special thanks to Marwadi University for their contribution to this project.

-  I would also like to acknowledge the support and guidance provided by Dr.Prof.Nishit Kotak Sir and Prof.Chandrasinh Parmar Sir.

---


