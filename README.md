# Generative AI for Video-to-Text Summarization

This repository contains the project **"Generative AI for Video-to-Text Summarization"**, completed as part of the CPTS 437 course. The goal of this project is to develop generative AI models that produce concise and accurate text summaries of instructional videos. We experimented with various LLMs, including FLAN-T5 and BART, and explored challenges in multimodal model integration.

---

## Project Description

### **Objective**
The aim is to generate accurate text summaries of instructional videos by leveraging state-of-the-art language models and techniques. We explored:
- Preprocessing video datasets for effective summarization.
- Fine-tuning pre-trained LLMs such as FLAN-T5 and BART.
- Comparing the empirical results from different models.
- Addressing multimodal challenges, including feature extraction and alignment.

### **Key Features**
- **Data Preparation**: Preprocessed datasets using YouTube instructional videos from the HowTo100M dataset.
- **Fine-Tuned Models**: Trained FLAN-T5 and BART on video captions to generate task summaries.
- **Evaluation Metrics**: Used ROUGE and BLEU scores to evaluate model performance.
- **Challenges**: Encountered and documented limitations in multimodal feature extraction.

---

## Deliverables

The following documents and materials summarize the project and its outcomes:

### 1. Project Proposal
- [Initial Project Proposal](Deliverables/CPTS_437_Project_Proposal.pdf)

### 2. Project Write-Up
- [Final Project Write-Up](Deliverables/Generative_AI_for_Video_to_Text_Summarization_Final_Report.pdf): This document includes the thought process, problem formulation, solution description, empirical insights, and results.

### 3. Presentation Materials
- [Presentation Slides](Deliverables/Generative_AI_for_Video_to_Text_Summarization_Presentation.pdf)

---

## Code and Demo

The code for the project is available in this repository. A detailed demo can be run using the provided Jupyter Notebooks.

### **Key Files**
- **Data Preprocessing**: [`Data_Preprocessing_Preparation.ipynb`](Data_Preprocessing_Preparation.ipynb)
- **FLAN-T5 Model Fine-Tuning**: [`Text_Generation_FLAN_T5.ipynb`](Text_Generation_FLAN_T5.ipynb)
- **BART Model Fine-Tuning**: [`Text_Generation_BART.ipynb`](Text_Generation_BART.ipynb)
- **Multimodal Learning (Scrapped)**: [`Multimodal_Learning.ipynb`](Multimodal_Learning.ipynb)

### **Run the Demo**
1. **Clone this repository**:
   ```bash
   git clone https://github.com/ethanvillalovoz/GenerativeAI-VideoSummarization.git
   cd GenerativeAI-VideoSummarization
   ```
2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```
3. **Run the notebooks**:
   * Open Data_Preprocessing_Preparation.ipynb to preprocess the dataset.
   * Fine-tune models using Text_Generation_FLAN_T5.ipynb or Text_Generation_BART.ipynb.

Here is a link to a Google Colab where you can demo and learn how to run our code: [Link](https://colab.research.google.com/drive/1QD04ii2pjK7tJ2RIA96OMbG7QyztThJG?usp=sharing)

## Results and Insights

### Evaluation Metrics

#### **FLAN-T5**
- **ROUGE-1**: Precision: 0.1799, Recall: 0.2112, F1: 0.1896
- **ROUGE-2**: Precision: 0.0415, Recall: 0.0448, F1: 0.0421
- **ROUGE-L**: Precision: 0.1797, Recall: 0.2109, F1: 0.1893
- **ROUGE-Lsum**: Precision: 0.1800, Recall: 0.2114, F1: 0.1897
- **BLEU**: 0.0
  - Precisions: [0.1801, 0.0415, 0.0, 0.0]
  - Brevity Penalty: 1.0
  - Length Ratio: 1.1375
  - Translation Length: 12,390
  - Reference Length: 10,892

#### **BART**
- **ROUGE-1**: Precision: 0.0355, Recall: 0.2377, F1: 0.0610
- **ROUGE-2**: Precision: 0.0068, Recall: 0.0503, F1: 0.0118
- **ROUGE-L**: Precision: 0.0353, Recall: 0.2370, F1: 0.0606
- **ROUGE-Lsum**: Precision: 0.0353, Recall: 0.2369, F1: 0.0607
- **BLEU**: 0.0017
  - Precisions: [0.0346, 0.0066, 0.0003, 0.0001]
  - Brevity Penalty: 1.0
  - Length Ratio: 6.8252
  - Translation Length: 74,340
  - Reference Length: 10,892

---

## Challenges

1. **GPU Memory**: Encountered limitations with 4 NVIDIA RTX A6000 GPUs during multimodal model integration.
2. **Multimodal Fusion**: This step was scrapped due to dimensionality mismatch in extracted features.

---

## Environment and Hardware

- **Environment**: Jupyter Notebooks in VS Code
- **Python Version**: 3.8.10
- **Hardware**: 4 NVIDIA RTX A6000 GPUs

---

## Questions or Feedback?

If you have any questions or feedback about this project, feel free to reach out at [ethanvillalovoz.github.io](https://ethanvillalovoz.github.io).

