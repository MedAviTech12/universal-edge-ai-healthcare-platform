# Universal Plug-and-Play Edge AI Platform for Multimodal Healthcare Diagnostics
![Project Status](https://img.shields.io/badge/Status-Completed-success)
![Platform](https://img.shields.io/badge/Platform-Raspberry%20Pi-blue)
![Domain](https://img.shields.io/badge/Domain-Healthcare%20AI-green)

This project presents a Universal Plug-and-Play Edge AI Platform for healthcare diagnostics. The platform enables the deployment and execution of multiple artificial intelligence models on a low-cost Raspberry Pi device, eliminating dependence on cloud-based infrastructure.

The system supports multimodal healthcare data, including facial images, thermal images, chest X-rays, respiratory audio recordings, and dermatological images. By performing inference locally on the edge device, the platform enhances data privacy, reduces latency, and improves accessibility in resource-constrained environments.

Designed with a modular architecture and dynamic model registry, the platform allows healthcare AI models to be integrated, updated, and deployed without modifying the core system. This enables scalable and flexible deployment across a wide range of healthcare applications.

## Table of Contents

- Key Features
- Project Overview
- Objectives
- System Architecture
- Healthcare AI Models Integrated
- Hardware and Software Stack
- Results and Performance
- Future Scope
- Documentation


## Key Features

- Plug-and-Play AI Model Deployment
- Edge Computing on Raspberry Pi
- Privacy-Preserving Local Inference
- Multimodal Healthcare Data Processing
- Dynamic Model Registry
- Real-Time AI Predictions
- Scalable and Modular Architecture

## Project Overview

Healthcare artificial intelligence systems often rely on cloud computing resources for model execution and data processing. While cloud-based solutions provide computational scalability, they may introduce challenges related to latency, internet dependency, operational costs, and patient data privacy.

To address these challenges, this project proposes a Universal Plug-and-Play Edge AI Platform capable of executing multiple healthcare AI models directly on a Raspberry Pi edge device. The platform enables real-time inference while keeping sensitive healthcare data local to the deployment environment.

The system is designed around a modular architecture that supports dynamic model integration through a centralized model registry. This allows healthcare AI models to be added, updated, or replaced without modifying the core application, making the platform scalable and adaptable for diverse healthcare applications.

The platform integrates multiple diagnostic and analytical models, including facial emotion recognition, thermal emotion detection, skin disease classification, tuberculosis detection from chest X-ray images, and tuberculosis screening using respiratory audio recordings.

## Objectives

The primary objective of this project was to develop a Universal Plug-and-Play Edge AI Platform capable of running multiple healthcare diagnostic models on a low-cost edge device.

Specific objectives include:

* Develop a unified platform for integrating multiple healthcare AI models.
* Enable real-time AI inference on Raspberry Pi hardware.
* Support multimodal healthcare data, including facial images, thermal images, chest X-rays, dermatological images, and respiratory audio recordings.
* Implement a dynamic model registry for plug-and-play model deployment.
* Reduce dependence on cloud infrastructure by performing local inference.
* Enhance patient privacy and data security through edge computing.
* Optimize AI models for resource-constrained environments using TensorFlow Lite.
* Create a scalable framework that allows new healthcare AI models to be added with minimal system modification.

## System Architecture
<img width="708" height="880" alt="image" src="https://github.com/user-attachments/assets/c21acdfc-dfc8-4045-8146-52524819f4bc" />


The proposed system follows a modular edge-computing architecture designed to support multiple healthcare AI applications on a single Raspberry Pi device. The architecture enables efficient data processing, dynamic model selection, and real-time inference while maintaining patient privacy through local execution.

### Architecture Workflow

User Input
      ↓
Data Preprocessing
      ↓
Model Registry
      ↓
Inference Engine
      ↓
AI Model Execution
      ↓
Prediction Output
      ↓
User Dashboard

### Core Components

#### 1. User Interface Layer

Provides a web-based dashboard that allows users to upload healthcare data, select AI models, and view prediction results.

#### 2. Data Preprocessing Layer

Processes incoming data according to its modality. The preprocessing pipeline includes image normalization, feature extraction, audio signal processing, and data validation before model execution.

#### 3. Model Registry

Acts as the central management system for all integrated AI models. The registry stores model metadata, preprocessing requirements, input specifications, and model locations, enabling plug-and-play deployment.

#### 4. Inference Engine

Loads the selected TensorFlow Lite model, executes inference on the edge device, and returns prediction results while optimizing memory and computational resource usage.

#### 5. AI Model Layer

The platform integrates multiple healthcare AI models, including:

* Facial Emotion Recognition
* Thermal Emotion Detection
* Skin Disease Classification
* Tuberculosis Detection from Chest X-Ray Images
* Tuberculosis Detection from Respiratory Audio

## Data Flow Diagram
<img width="977" height="482" alt="image" src="https://github.com/user-attachments/assets/96444dd7-1852-480a-a32e-55024cfe056f" />


#### 6. Edge Hardware Layer

The entire system is deployed on a Raspberry Pi 4 device, enabling local processing, reduced latency, and privacy-preserving healthcare diagnostics.

## Healthcare AI Models Integrated


| Model                                      | Application Area                                |
| ------------------------------------------ | ----------------------------------------------- |
| Facial Emotion Recognition                 | Emotion Analysis from Facial Images             |
| Thermal Emotion Detection                  | Emotion Recognition using Thermal Facial Images |
| Skin Disease Classification                | Dermatological Disease Screening                |
| Tuberculosis Detection (Chest X-Ray)       | Pulmonary Tuberculosis Screening                |
| Tuberculosis Detection (Respiratory Audio) | Audio-Based Tuberculosis Screening              |

The platform integrates multiple healthcare AI models within a unified edge-computing framework. Each model is optimized for deployment on resource-constrained hardware and can be dynamically selected through the model registry system without modifying the platform architecture.

## Hardware and Software Stack

### Hardware

| Component        | Specification                |
| ---------------- | ---------------------------- |
| Edge Device      | Raspberry Pi 4 Model B       |
| Processor        | Quad-core ARM Cortex-A72 CPU |
| Memory           | 8 GB RAM                     |
| Storage          | SD Card / External Storage   |
| Input Devices    | Camera, Microphone           |
| Operating System | Raspberry Pi OS (Linux)      |

### Software

| Category                   | Technologies                        |
| -------------------------- | ----------------------------------- |
| Programming Language       | Python                              |
| Machine Learning Framework | TensorFlow, TensorFlow Lite         |
| Web Framework              | Flask                               |
| Image Processing           | OpenCV                              |
| Numerical Computing        | NumPy                               |
| Frontend Development       | HTML, CSS, JavaScript               |
| Deployment Environment     | Linux-based Edge Computing Platform |

### Development Tools

* TensorFlow / Keras
* TensorFlow Lite Converter
* OpenCV
* NumPy
* Flask Framework
* Raspberry Pi OS

## Hardware Integration 
<img width="959" height="1034" alt="image" src="https://github.com/user-attachments/assets/55297eab-3386-4072-8d61-7594999de5b9" />

## Results and Performance

The proposed Edge AI platform was successfully deployed and evaluated on a Raspberry Pi 4 device. Experimental testing demonstrated the feasibility of running multiple healthcare AI models locally while maintaining acceptable inference speed and resource efficiency.
## Web Dashboard
<img width="1541" height="1202" alt="image" src="https://github.com/user-attachments/assets/88f260a7-e201-49df-aca3-2aea14c8e8ed" />

### Key Achievements

* Successfully integrated five healthcare AI models into a unified platform.
* Implemented dynamic plug-and-play model deployment through a centralized model registry.
* Enabled real-time healthcare inference on Raspberry Pi hardware.
* Reduced model size through TensorFlow Lite optimization for edge deployment.
* Supported multimodal healthcare data, including images, thermal data, and audio recordings.

### Model Size Optimization

| Model                            | Original Size | TFLite Size | Reduction |
| -------------------------------- | ------------- | ----------- | --------- |
| Facial Emotion Recognition       | 67.2 MB       | 17.1 MB     | 74.6%     |
| Skin Disease Classification      | 54.8 MB       | 14.3 MB     | 73.9%     |
| Thermal Emotion Detection        | 13.6 MB       | 3.5 MB      | 74.3%     |
| TB Detection (Chest X-Ray)       | 102.4 MB      | 26.1 MB     | 74.5%     |
| TB Detection (Respiratory Audio) | 18.3 MB       | 1.8 MB      | 90.2%     |

### Average Inference Latency

| Model                            | Total Latency |
| -------------------------------- | ------------- |
| Facial Emotion Recognition       | 364 ms        |
| Skin Disease Classification      | 405 ms        |
| Thermal Emotion Detection        | 384 ms        |
| TB Detection (Chest X-Ray)       | 505 ms        |
| TB Detection (Respiratory Audio) | 374 ms        |

The experimental results demonstrate that multiple healthcare AI applications can be deployed efficiently on resource-constrained edge devices while maintaining practical response times for real-world healthcare scenarios.

## Future Scope

The proposed Edge AI platform establishes a foundation for scalable and privacy-preserving healthcare diagnostics. Several enhancements can be explored in future work to improve system functionality, clinical applicability, and deployment readiness.

### Potential Future Enhancements

* Integration of additional healthcare AI models for disease detection and patient monitoring.
* Support for Internet of Things (IoT) and wearable medical devices for real-time health data acquisition.
* Development of a mobile application for remote access and monitoring.
* Implementation of federated learning to enable collaborative model improvement while preserving data privacy.
* Integration with electronic health record (EHR) systems for seamless clinical workflow support.
* Optimization for lower-power embedded devices and edge accelerators.
* Expansion of multimodal analysis capabilities through the integration of additional physiological signals.
* Clinical validation through large-scale testing in real-world healthcare environments.

### Long-Term Vision

The long-term goal of this project is to develop a flexible and scalable Edge AI ecosystem capable of delivering accessible, privacy-preserving, and real-time healthcare intelligence in hospitals, rural healthcare centers, and resource-constrained environments.

## Documentation

The repository contains the following project resources:

- Final Year Project Report
- Project Presentation
- System Architecture Diagrams
- Experimental Results and Performance Analysis
- Deployment and Implementation Details

## Author

**Abhishek Kumar Jha**

Biomedical Engineering Graduate

Areas of Interest:
- Medical Artificial Intelligence
- Neuroengineering
- Medical Imaging
- Edge AI
- Intelligent Healthcare Systems

LinkedIn: https://www.linkedin.com/in/abhishek-kumar-jha-027a13263/
GitHub: https://github.com/MedAviTech12
