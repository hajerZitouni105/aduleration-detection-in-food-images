# Food Adulteration Detection from Images Using CNN and Autoencoder Architectures

## About
This project uses deep learning to detect food adulteration through two distinct models:

- **CNN-based Classification** for binary classification of images as either authentic or adulterated.
- **Autoencoder-based Anomaly Detection** for unsupervised anomaly detection, flagging adulterated samples based on reconstruction error.

Both models target specific datasets: a **Meat Adulteration Dataset** and a **Pistachio Adulteration Dataset**, available on Kaggle.

## Project Structure
- **Pistachio adulteration**:  focusing on CNN classification.
- **Meat adulteration**: for the autoencoder anomaly detection approach.

## Datasets
We used two food adulteration datasets from Kaggle:

- **Meat Adulteration Dataset**
- **Pistachio Adulteration Dataset**

Each dataset includes labeled images, enabling binary classification and anomaly detection.

## Methodologies

### CNN Classification Methodology
The CNN model workflow includes:

1. **Data Preprocessing**: Resizing, normalization, and augmentation to balance classes and increase robustness.
2. **Model Architecture**: CNN designed to capture key visual features that distinguish authentic and adulterated samples.
3. **Training and Evaluation**: The model is trained and evaluated on metrics like accuracy and precision.

### Autoencoder Anomaly Detection Methodology
The autoencoder workflow includes:

1. **Data Augmentation**: The meat dataset was initially augmented to increase sample diversity.
2. **Training on Authentic Images**: The autoencoder is trained solely on authentic images, learning to reconstruct these with minimal error.
3. **Anomaly Detection via Reconstruction Error**: After training, any image producing a high reconstruction error is flagged as potentially adulterated.
4. **Final Evaluation**: Reconstruction errors are analyzed, and an error threshold is set to optimize detection accuracy.

## Installation and Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/food-adulteration-detection.git
## Results
- **CNN Classifier:** Achieved strong performance in classifying adulterated vs. authentic samples.
- **Autoencoder:** Successfully detected adulteration by identifying samples with higher reconstruction errors.

## Future Directions
- **Broader Dataset Inclusion:** Explore more types of food adulteration.
- **Deployment:** Adapt the models for real-time use on mobile or web applications.
