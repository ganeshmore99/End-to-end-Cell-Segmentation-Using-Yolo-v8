# End-to-End Cell Segmentation Using YOLO v8

## Introduction

This project demonstrates the complete process of implementing an end-to-end cell segmentation system using the YOLO v8 architecture. The repository covers all the necessary steps from setting up the project to deploying the model on Azure Cloud.

## Table of Contents

#### Introduction and GitHub Repository Setup
#### Project Template Creation
#### What is Object Segmentation
#### Introduction to YOLO v8
#### Project Setup and Requirements Installation
#### Logging, Utils, and Exceptions Modules
#### Project Workflows
#### Data Annotation (Polygon)
#### Notebook Research
#### YOLO v8 Setup
#### Modular Code Implementation
#### Training Pipeline
#### Prediction Pipeline and User App Creation
#### Docker
#### GitHub Actions
#### Final CI/CD Deployment on Azure Cloud

## Introduction and GitHub Repository Setup
Start by creating a new GitHub repository and cloning it to your local machine. Initialize a README file and set up the basic directory structure.

## Project Template Creation
Design a project template that includes all necessary folders and files such as src, data, notebooks, and configuration files.

## What is Object Segmentation
Object segmentation is a computer vision task where the goal is to identify and delineate each object in an image at a pixel level. Unlike object detection, which only provides bounding boxes, segmentation provides precise boundaries.

## Introduction to YOLO v8
YOLO (You Only Look Once) v8 is the latest version of the YOLO family. It is a state-of-the-art, real-time object detection and segmentation algorithm known for its speed and accuracy.

## Project Setup and Requirements Installation
Set up your project environment and install all necessary dependencies. Create a requirements.txt file for easy installation of packages.

pip install -r requirements.txt

## Logging, Utils, and Exceptions Modules
Implement logging to track the application's behavior, utility functions for common tasks, and exception handling to manage errors gracefully.

## Project Workflows
Outline the workflows for data preprocessing, model training, and inference. Define clear steps and processes for each workflow.

## Data Annotation (Polygon)
Use polygon annotation tools to label the cells in your dataset. Save the annotations in a format that can be used for training the YOLO v8 model.

## Notebook Research
Conduct initial experiments and research in Jupyter notebooks. Document your findings and insights which will guide the development of the modular code.

## YOLO v8 Setup
Download and set up the YOLO v8 model. Configure the model for cell segmentation tasks by adjusting the configuration files.

## Modular Code Implementation
Refactor the research code into modular, reusable components. Ensure that each module has a single responsibility and can be tested independently.

## Training Pipeline
Develop a training pipeline to train the YOLO v8 model on your annotated dataset. Include steps for data loading, augmentation, model training, and evaluation.

## Prediction Pipeline and User App Creation
Create a prediction pipeline to make inferences on new data. Develop a user-friendly application to allow users to upload images and view segmentation results.

## Docker
Dockerize the application to ensure a consistent environment across different machines. Create a Dockerfile and set up Docker Compose if necessary.

## GitHub Actions
Set up GitHub Actions for continuous integration. Configure workflows to run tests, build the Docker image, and deploy the application automatically.

## Final CI/CD Deployment on Azure Cloud
Deploy the final application on Azure Cloud using the CI/CD pipeline configured with GitHub Actions. Ensure that the deployment is seamless and scalable.

## Workflows

1. constants
2. entity
3. components
4. pipelines
5. app.py


# How to run?
### STEPS:

Clone the repository

```bash
https://github.com/ganeshmore99/End-to-end-Cell-Segmentation-Using-Yolo-v8.git
```
### STEP 01- Create a conda environment after opening the repository

```bash
conda create -n cell python=3.8 -y
```

```bash
conda activate cell
```


### STEP 02- install the requirements
```bash
pip install -r requirements.txt
```


```bash
# Finally run the following command
python app.py
```

Now,
```bash
open up you local host and port
```


# AZURE-CICD-Deployment-with-Github-Actions

## Save pass:

S6tXzK7IxUHz9O/9jkhciLsseddeQ++E+OcD7nQYy8+ACRDtEgUW

## Run from terminal:

docker build -t cellseg.azurecr.io/cell:latest .

docker login cellseg.azurecr.io

docker push cellseg.azurecr.io/cell:latest


## Deployment Steps:

1. Build the Docker image of the Source Code
2. Push the Docker image to Container Registry
3. Launch the Web App Server in Azure 
4. Pull the Docker image from the container registry to Web App server and run 


## Contributing
Contributions are welcome! Please read the contribution guidelines before making a contribution.

## License
This project is licensed under the MIT License. See the LICENSE file for more details.

## Acknowledgments
Thank you to everyone who contributed to this project. Special thanks to the authors and maintainers of the YOLO v8 framework.
