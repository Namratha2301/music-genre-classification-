# Music Genre Classification using Federated Learning

Paper Link: https://link.springer.com/chapter/10.1007/978-981-19-7447-2_23
<img width="533" alt="Screenshot 2024-11-05 at 10 46 36 PM" src="https://github.com/user-attachments/assets/438509d5-48b4-42c6-84ea-727c54608611">
<img width="412" alt="Screenshot 2024-11-05 at 10 46 42 PM" src="https://github.com/user-attachments/assets/cde478e4-035a-41dd-a524-06db81d8ecd3">


# Music Genre Classification Using Federated Learning

This project leverages Federated Learning (FL) to perform music genre classification on audio data without compromising user data privacy. FL allows machine learning models to train on decentralized data without requiring the data to be shared with a central server. This approach is especially relevant for the music industry, where privacy concerns are high, as it enables collaboration across entities while keeping sensitive data secure.

## Key Details

- **Dataset**: Utilizes the GTZAN music genre dataset, containing 10 genres (e.g., rock, jazz, hip-hop, etc.), with each genre having an equal distribution of 1000 samples.
- **Model Architecture**: Employs a Convolutional Neural Network (CNN) with four convolutional layers followed by dense layers, which effectively extracts features from audio spectrograms for genre classification.
- **Federated Learning Approach**: Implements a centralized FL architecture where local client updates are aggregated on a central server using the Federated Averaging (FedAvg) algorithm, ensuring privacy and reducing data storage needs.
- **Data Processing**: Audio files are split into smaller segments, converted into grayscale spectrograms, and further optimized for FL. TensorFlow Federated is used to handle client-server interactions and simulate real-world federated data distribution.
- **Results**: The FL model achieves accuracy levels comparable to traditional centralized models, providing strong performance while enhancing data privacy and autonomy.

## Key Contributions

1. Demonstrates decentralized training for music genre classification.
2. Ensures data privacy by keeping audio data on local devices.
3. Validates FL’s feasibility for audio data applications in the music industry.

## Technologies Used

- **Libraries**: TensorFlow Federated, Keras
- **Algorithms**: FedAvg for model aggregation, CNN for feature extraction

## Results Comparison

| S.No | Model Comparison                   | Training Approach             | Training Accuracy | Testing Accuracy |
|------|------------------------------------|-------------------------------|-------------------|------------------|
| 1    | Proposed Federated Learning        | Without scaling               | 80.2%            | 76.02%          |
| 2    | Proposed Federated Learning        | With 25% scaling              | 76.46%           | 71.78%          |
| 3    | Centralized (Neural Network) Model | Traditional centralized model | 92.84%           | 81.65%          |

The federated approach shows competitive accuracy compared to the centralized model, highlighting its viability as a privacy-preserving alternative for real-world applications.

---

This project provides a secure and scalable solution for collaborative machine learning in music genre classification, offering potential applications across privacy-sensitive domains.
