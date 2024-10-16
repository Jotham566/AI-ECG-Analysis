# AI-Enabled Electrocardiogram (ECG) Analysis for Small Japanese Clinics

## Project Overview
This project leverages deep neural networks (DNNs) to enhance electrocardiogram (ECG) interpretation for small, resource-constrained clinics in Japan. The primary aim is to improve the accuracy and accessibility of cardiovascular disease (CVD) detection, particularly in rural areas with limited specialist access.

## Key Objectives
1. **Quantify the impact of visual ECG inspection** for CVD diagnosis.
2. **Develop and evaluate** a deep learning model tailored for small clinics to enhance ECG interpretation.
3. **Define market potential, early adopter profile, and value proposition** for AI-enabled ECG analysis.
4. **Formulate an implementation plan** addressing adoption barriers like cost, technical infrastructure, and trust.

## Key Outcomes
- **Model Accuracy**: Achieved 98.46% accuracy across 11 cardiac conditions, outperforming human experts (83.4%).
- **Efficiency**: Reduced ECG analysis time from minutes to seconds.
- **Cost-Effectiveness**: Designed for small clinics without requiring expensive ECG devices.

## Methodology
- **Dataset**: 45,152 12-lead ECG recordings from the [PhysioNet](https://physionet.org/content/ecg-arrhythmia/1.0.0/) database.
- **Model**: Built using Bidirectional GRU layers, multi-head attention, and global average pooling.
- **Class Imbalance Handling**: SMOTE and RENN techniques were used for class balancing.

## Model Architecture
- **Input**: 12-lead ECG data, reshaped to (200, 300).
- **Layers**:
  - Bidirectional GRU (512 units each).
  - Multi-head attention (13 heads).
  - Global average pooling.
  - Dense (11 units, softmax).

## Performance Metrics
- **Test Accuracy**: 98.46%
- **Macro F1-score**: 0.9819
- **Precision Range**: 0.972 - 0.992
- **Recall Range**: 0.900 - 0.999

## Challenges Addressed
- **Limited Specialist Access**: Designed to assist in rural areas with high CVD prevalence and limited specialists.
- **High Human Error Rates**: AI model significantly reduces error rates that ranged from 36-96% in human ECG interpretation.
- **Adoption Barriers**: Addressed issues related to cost, system integration, data privacy, and trust in AI.

## Future Work
1. Expand the model to integrate multimodal data (e.g., patient history, lifestyle).
2. Develop predictive analytics for personalized preventive care.
3. Launch a startup to commercialize the AI-enabled ECG solution.

## How to Run
1. Clone the repository.
2. Install dependencies using `requirements.txt`.
3. Open and run the provided Preprocessing Jupyter notebook `preprocessing.ipynb` to execute the preprocessing steps.
4. Ensure access to the dataset from [PhysioNet](https://physionet.org/content/ecg-arrhythmia/1.0.0/).

---

## Contact
For questions & Model Architecture Notebook, contact Jotham Wambi: jothammartin.wambi@gmail.com
