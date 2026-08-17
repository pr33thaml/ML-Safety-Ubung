# Machine Learning Safety – Exercises

**Otto-von-Guericke University Magdeburg (OvGU)**
**Course:** Introduction to Machine Learning Safety
**Semester:** Summer 2026
**Author:** Preetham Louis

## About

This repository contains the exercises and notebooks completed for the **Introduction to Machine Learning Safety** course at Otto-von-Guericke University Magdeburg.

The exercises use a **CARLA autonomous driving perception system** to investigate different aspects of machine learning **safety, security, robustness, explainability, and uncertainty**.

The perception system consists of three binary classifiers:

* 🚶 **Pedestrians**
* 🚗 **Vehicles**
* 🚦 **Traffic Lights**

The classifiers use an **ImageNet-pretrained ResNet-18** backbone and forward-facing camera images from the CARLA simulator.

## Exercises

| Exercise | Topic                         | Description                                                                                                                                                            |
| -------- | ----------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **3**    | Model Training                | Training pedestrian, vehicle, and traffic-light classifiers. Covers model architecture, dataset preparation, and training configuration.                               |
| **4**    | Model Evaluation              | Evaluation using precision, recall, confusion matrices, and other classification metrics on clean test data.                                                           |
| **5**    | Backdoor Poisoning            | Investigation of backdoor attacks by modifying training data with a trigger and analysing their impact on model behaviour.                                             |
| **6**    | Explainability                | Analysis of model predictions using **Grad-CAM** and saliency maps.                                                                                                    |
| **7**    | Out-of-Distribution Detection | Detection of inputs outside the training distribution, including fog, nighttime, and different CARLA towns. Uses **MSP** and feature-based **k-NN** anomaly detection. |
| **8**    | Adversarial Machine Learning  | Evaluation of model robustness against adversarial perturbations using **FGSM**.                                                                                       |
| **9**    | Uncertainty & Calibration     | Evaluation of model confidence using **ECE**, temperature scaling, and cost-sensitive decision thresholds.                                                             |

## Repository Structure

```text
.
├── exercise3/    # Model training
├── exercise4/    # Model evaluation
├── exercise5/    # Backdoor poisoning
├── exercise6/    # Explainability
├── exercise7/    # Out-of-distribution detection
├── exercise8/    # Adversarial machine learning
└── exercise9/    # Uncertainty and calibration
```

## Requirements

The notebooks are implemented using **Python**, **PyTorch**, and **Jupyter Notebook**.

### Main Dependencies

* [PyTorch](https://pytorch.org/)
* [Torchvision](https://pytorch.org/vision/)
* [NumPy](https://numpy.org/)
* [Pandas](https://pandas.pydata.org/)
* [Matplotlib](https://matplotlib.org/)
* [Scikit-learn](https://scikit-learn.org/)
* [NetCal](https://github.com/EFS-OpenSource/calibration-framework)
* [Grad-CAM](https://github.com/jacobgil/pytorch-grad-cam)

### Installation

Install the required packages with:

```bash
pip install torch torchvision numpy pandas matplotlib scikit-learn netcal grad-cam
```

## Topics Covered

The repository covers several important areas of machine learning safety:

* Model training and evaluation
* Backdoor attacks and data poisoning
* Model explainability
* Out-of-distribution detection
* Adversarial robustness
* Uncertainty estimation
* Model calibration
* Cost-sensitive classification

## Disclaimer

This repository contains coursework completed as part of the **Introduction to Machine Learning Safety** course at Otto-von-Guericke University Magdeburg. It is intended for educational and research purposes.
