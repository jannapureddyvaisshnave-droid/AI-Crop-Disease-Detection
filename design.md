# System Design Document

## 1. System Architecture Overview
The system uses a simple client-server architecture where a lightweight AI model trained using Google Teachable Machine is used to classify crop leaf images and provide instant feedback to users.

## 2. High-Level Architecture
- User Interface: Simple mobile or web interface
- AI Model: Image classification model trained using Teachable Machine
- Inference Layer: TensorFlow.js or exported model
- Storage: Minimal logging for analysis

## 3. Component Description

### 3.1 User Interface
- Allows image capture or upload
- Displays classification results
- Designed for non-technical users

### 3.2 AI Model
- Image classification model trained on leaf images
- Created using Google Teachable Machine
- Exported for web or mobile inference
- Lightweight and fast

### 3.3 Inference Engine
- Uses TensorFlow.js to run the model
- Performs real-time predictions
- Requires minimal computing resources

## 4. Data Flow
1. User uploads or captures a leaf image
2. Image is processed locally or sent for inference
3. AI model predicts the class (healthy/diseased)
4. Result is shown to the user

## 5. Model Training
- Image collection for healthy and diseased leaves
- Training performed using Google Teachable Machine
- Model exported for deployment

## 6. Technology Stack
- Frontend: HTML/CSS/JavaScript or simple mobile UI
- AI/ML: Google Teachable Machine + TensorFlow.js
- Backend: Optional (for logging or updates)
- Hosting: Cloud or local hosting

## 7. Responsible AI Considerations
- Display confidence scores with predictions
- Encourage consulting experts for severe cases
- Avoid over-reliance on AI outputs

## 8. Scalability & Deployment
- Lightweight deployment suitable for multiple users
- Easy retraining with new images
- Low infrastructure cost

## 9. Future Enhancements
- Support for more crop types
- Multi-language support
- Offline inference support
