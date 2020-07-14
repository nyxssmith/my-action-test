# SFL Scientific Project Tamplete

<p align="center"><img width=50% src="imgs/logo.png"></p>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;

![Python](https://img.shields.io/badge/python-v3.6+-blue.svg)
[![Build Status](https://travis-ci.org/anfederico/Clairvoyant.svg?branch=master)](https://travis-ci.org/anfederico/Clairvoyant)
![Dependencies](https://img.shields.io/badge/dependencies-up%20to%20date-brightgreen.svg)

## Purpose (filled out at beginning)

- The purpose of this project is ________.
- Describe the main goals of the project and potential business impact.
- Limit to a short paragraph, 3-6 Sentences.

## Project Description (filled out at beginning)

given A, B,C the program do X, Y,Z and output 1,2 ,3

- H2: Data
    - Describe the data sufficiently for other developers to understand contents and limitations
- H2: Output
    - Describe the expected output

Index
=====
## Table of Contents
1. [Deployment](#1-Deployment)\
	1.1 [Environment Dependencies](#11-Environment-Dependencies)\
    1.2 [Docker Registry Dependencies](#12-Docker-Registry-Dependencies)\
    1.3 [Data Dependencies](#13-Data-Dependencies)\
    1.4 [Installation](#14-Installation)
2. [Usage](#2-Usage)\
	2.1 [Training Usage](#21-Training-Usage)\
    2.2 [Inference Usage](#22-Inference-Usage)\
    2.3 [Configuration](#23-Configuration)\
    2.4 [Training Validation](#24-Training-Validation)
3. [Project Contents](#3-Project-Contents)
4. [Notes](#4-Notes)
5. [Known Issues](#5-Known-Issues)
6. [Contacts](#6-Contacts)


## 1. Deployment
([Return to Table of Contents](#Table-of-Contents))
### 1.1 Environment Dependencies

(filled out when end-to-end testing commences) 

- The required enviroment of this project is A,B,C.
- Describe the environment dependencies with external link.
    - e.g: Upgrade Docker to at least version 19.03. If using older docker versions then install NVIDIA container toolkit [NVIDIA toolkit install](https://github.com/NVIDIA/nvidia-docker/blob/master/README.md)
- Limit to a short paragraph, 3-6 Sentences.


### 1.2 Docker Registry Dependencies

(filled out when end-to-end testing commences) 

- The docker registry address is ________.
- The docker registry credential is ________.
- Instruction to login registry: ________.

### 1.3 Data Dependencies

(filled out when end-to-end testing commences) 

* For training, the input data is ________, which is A/B/C in configuration section X/Y/Z.
* For inference, the input data is ________, which is A/B/C in configuration section X/Y/Z.
- Describe the input data/external data dependencies(e.g: pretrained model weight) for each functionality.

### 1.4 Installation

(filled out when end-to-end testing commences) 

* To install the program, run ________.
- Describe the necessary steps(e.g: docker build/run) to install the program.


## 2. Usage
([Return to Table of Contents](#Table-of-Contents))

Information on each feature provided by your application, these may vary from the following example subsections.

### 2.1 Training Usage

(filled out when end-to-end testing commences) 

Overall, the training pipeline does ________.
To run the training pipeline, run ________.
- Describe the necessary steps(e.g: docker build/run) to run training pipeline.
- For data dependencies, specify which configuration in which configuration file need to be updated.

### 2.2 Inference Usage

(filled out when end-to-end testing commences) 

Overall, the inference pipeline does ________.
To run the inference pipeline, run ________.
- Describe the necessary steps(e.g: docker build/run) to run inference pipeline.
- For data dependencies, specify which configuration in which configuration file need to be updated.

### 2.3 Configuration

(filled out when end-to-end testing commences) 

- Describe the **configurations that is expected to change in future only**.

#### Training Configuration

##### Section A

* XXX
* XXX

##### Section B

* XXX

#### Inference Configuration

##### Section A

* XXX
* XXX

##### Section B

* XXX

### 2.4. Training Validation

Overview: fill me

To run:

1. fill me
2. fill me

### 3. Project Contents
([Return to Table of Contents](#Table-of-Contents))

    ├── LICENSE
    ├── README.md          <- The top-level README for developers using this project.
    ├── run.sh             <- Bash script to run main function. Main function includes training, inference and QA testing.
    ├── data
    │   ├── external       <- Data from third party sources.
    │   ├── interim        <- Intermediate data that has been transformed.
    │   ├── processed      <- The final, canonical data sets for modeling. Data pipeline output data should be saved in this folder.
    │   └── raw            <- The original, immutable data dump. Raw input data should be saved in this folder
    │
    ├── docs               <- Presentations and reports.
    │
    ├── models             <- Trained and serialized models, model predictions, or model summaries
    │
    ├── notebooks
    │   └── [Prod]<YOUR-NOTEBOOK>.md        <- Your data science NoteBook
    │
    ├── src                <- Source code for use in this project.
    │   │
    │   ├── train.py             <- Train program main script: your training pipeline should go into this script.
    │   ├── predict.py           <- Inference program main function: your inference pipeline should go into this script.
    │   │
    │   ├── datasets           <- Scripts to download or generate data: your dataset related code should go into this folder.
    │   │   └── dataset1.py: Script for data IO and processing
    │   │   └── dataset2.py: Script for data IO and processing
    │   │
    │   ├── models         <- Scripts to train models and then use trained models to make
    │   │   │                 predictions
    │   │   ├── builder.py: Script for Model builder. Your model initialization code should go into this script.
    │   │   └── model.py: Script for your model structure. Your model structure code should go into this script.
    │   │   └── trainer.py: Script for model training. Your model training logic should go into this script.
    │   │
    │   ├── preprocesses           <- Scripts to process XXX data
    │   │   └── process.py: data preprocessing main object: update it when you works your own SFL project.
    │   │   └── transform.py: Transforms used in the image preprocessing pipeline: update it when you works your own SFL project.
    │   ├── postprocesses           <- Scripts to process XXX data
    │   │   └── process.py: data postprocessing main object: update it when you works your own SFL project.
    │   │   └── transform.py: Transforms used in the image postprocessing pipeline: update it when you works your own SFL project.
    │   ├── validation           <- Scripts to validate
    │   │   └── validate1.py: fill me
    │   │   └── validate2.py: fill me
    │   ├── netty           <- netty helper functions: includes commonly-used visualization and data split functions.
    ├── tests                <- scrips for QA/QC tests.
    │   │
    │   ├── test_train.py: integration test for your training pipeline: update it when you works your own SFL project.
    │   ├── test_predict.py: integration test for your inference pipeline: update it when you works your own SFL project.
    │   │
    │   ├── datasets           <- Unite test for your dataset objects: update it when you works your own SFL project.
    │   │   └── test_dataset1.py: Script for data IO and processing
    │   │   └── test_dataset2.py: Script for data IO and processing
    │   │
    │   ├── models         <-  Unite test for your builder/model/trainer objects: update it when you works your own SFL project.
    │   │   ├── test_builder.py: Model builder
    │   │   └── test_model.py: Script for your model structure.
    │   │   └── test_trainer.py: Script for model training.
    │   │
    │   ├── processes           <- Unite test for your data pipeline objects: update it when you works your own SFL project.
    │   │   └── test_preprocess.py: data preprocessing main object
    │   │   └── test_transform.py: Transforms used in the image preprocessing pipeline
    │   ├── validation           <- Unite test for your validation pipeline objects: update it when you works your own SFL project.
    │   │   └── test_validate1.py: fill me
    │   │   └── test_validate2.py: fill me

### 4. Notes
([Return to Table of Contents](#Table-of-Contents))\
(filled out when end-to-end testing commences)

### 5. Known Issues
([Return to Table of Contents](#Table-of-Contents))\
(filled out when end-to-end testing commences)

### 6. Contacts
([Return to Table of Contents](#Table-of-Contents))

    - Developers
    - SFL Scientific founders (Mike, Mike, Dan)