# Robust Vision Transformer for Violence Detection

## Overview

This repository accompanies the research work titled **“Robust Vision Transformer Framework for Low-False-Alarm Violence Detection in Real-World Surveillance.”**

The project investigates a Vision Transformer (ViT)-based approach to violence detection in surveillance videos, with an emphasis on reducing false alarms and improving the reliability of automated video analysis in real-world settings.

Violence detection in surveillance footage is challenging because aggressive and non-aggressive activities can share similar visual patterns. Changes in lighting, camera viewpoints, background activity, occlusion, and crowded scenes can further complicate classification. This project explores the use of transformer-based visual representations to support automated violence recognition.

## Objectives

- Develop a Vision Transformer-based framework for video violence detection.
- Investigate methods for reducing false-positive violence predictions.
- Evaluate classification performance using appropriate metrics.
- Examine the suitability of the framework for real-world surveillance scenarios.
- Support reproducible research through organized source code, configuration files, and evaluation procedures.

## Methodology

The proposed framework is designed around the following general workflow:

1. **Video data preparation:** Organize and preprocess the video data according to the selected dataset protocol.
2. **Frame sampling and preprocessing:** Extract representative frames and apply the preprocessing required by the model.
3. **Visual feature representation:** Use a Vision Transformer to learn informative visual representations.
4. **Violence classification:** Generate predictions for violence and non-violence classes using the implemented classification component.
5. **Evaluation:** Assess the model using classification metrics, including precision, recall, F1-score, and false-positive rate, where applicable.
6. **False-alarm analysis:** Examine incorrect violence predictions to understand the model's reliability in surveillance scenarios.

*Note: The workflow should be updated to match the final implemented architecture and experimental protocol.*

## Repository Structure

```text
robust-vit-violence-detection/
├── README.md
├── requirements.txt
├── configs/
├── data/
│   └── README.md
├── src/
│   ├── preprocessing.py
│   ├── model.py
│   ├── train.py
│   ├── evaluate.py
│   └── inference.py
├── notebooks/
├── results/
└── LICENSE
```

The structure above is a suggested organization. Include only files and modules that are actually implemented in the repository.

## Dataset

The framework is intended for evaluation on an appropriate violence-detection video dataset.

Before running the experiments:

- Obtain the dataset from its authorized source.
- Follow the dataset's licensing and usage conditions.
- Arrange the video files according to the expected directory structure.
- Apply the documented training, validation, and testing split.
- Avoid sharing restricted video data or personally identifiable information without authorization.

Dataset names, download instructions, and split details should be added once the exact experimental dataset has been confirmed.

## Installation

Clone the repository:

```bash
git clone https://github.com/<YOUR-USERNAME>/robust-vit-violence-detection.git
cd robust-vit-violence-detection
```

Create and activate a Python virtual environment:

```bash
python -m venv .venv
```

Install the dependencies:

```bash
pip install -r requirements.txt
```

The required Python version, framework versions, and hardware requirements should be specified based on the actual implementation.

## Usage

### Training

After configuring the dataset paths and model settings, run the training script:

```bash
python src/train.py
```

### Evaluation

Evaluate a trained model using the configured test set:

```bash
python src/evaluate.py
```

### Inference

Run inference on an eligible input video:

```bash
python src/inference.py
```

These commands are templates and should be adjusted to match the actual scripts, arguments, and checkpoints provided in the repository.

## Evaluation Metrics

The following metrics are relevant to assessing violence-detection performance:

- **Accuracy:** Overall proportion of correctly classified samples.
- **Precision:** Proportion of predicted violence cases that are actual violence cases.
- **Recall:** Proportion of actual violence cases correctly identified.
- **F1-score:** Harmonic mean of precision and recall.
- **False-positive rate (FPR):** Proportion of non-violence samples incorrectly classified as violence.

For surveillance applications, the false-positive rate should be considered alongside recall and detection latency. A low false-positive rate alone does not establish reliable detection if actual violence events are frequently missed.

## Experimental Results

Add the final results reported in the manuscript, including:

- Dataset and evaluation protocol.
- Comparison methods or baseline models.
- Accuracy, precision, recall, and F1-score.
- False-positive rate and its calculation method.
- Computational requirements and inference latency, if measured.

Only experimentally verified results should be reported. No performance values are included here because they have not been supplied for this README.

## Reproducibility

For reproducible experiments, document the following:

- Random seeds and software versions.
- Dataset splits and preprocessing settings.
- Model configuration and training hyperparameters.
- Checkpoint selection criteria.
- Evaluation scripts and metric definitions.
- Hardware used for training and inference.

## Limitations and Responsible Use

Automated violence detection can produce false alarms or miss genuine events. Predictions should not be treated as definitive evidence of violent behavior. Any deployment in surveillance settings should include appropriate human review, privacy safeguards, and evaluation across diverse environments.

## Citation

If you use this repository in academic work, cite the associated paper once its publication details are available.

**Manuscript title:** Robust Vision Transformer Framework for Low-False-Alarm Violence Detection in Real-World Surveillance

Author names, publication venue, DOI, and BibTeX citation can be added after the manuscript's bibliographic details are finalized.

## License

Specify an appropriate open-source license after confirming the licensing requirements for the code and any third-party components. Dataset licenses remain applicable independently of the repository license.

## Contact

For research-related questions, contact the corresponding author:

**Thulasi Bikku**  
Department of Computer Science and Engineering  
Amrita Vishwa Vidyapeetham, Amaravati, India  
Email: b_thulasi@av.amrita.edu
