# Model Card

## Model date
April 2024

## Model type
ConvNet (CNN)

## Model version
1.0

## Developer:
Aashima Arora

## Model Description

**Input:** 
The input to the model is a 192x192 RGB image representing a skin lesion. Each image contains three channels corresponding to red, green, and blue color intensities.

<img width="327" alt="input" src="https://github.com/aashimarora/IMPL-Project-AIDerm/assets/21965720/0e0d6330-fa4c-46de-80c0-00c1451a8138">


**Output:** 
The output of the model is a probability distribution over the classes of skin lesions present in the input image. The model predicts the likelihood of each class, including but not limited to melanoma, psoriasis, eczema, and acne.

<img width="326" alt="output" src="https://github.com/aashimarora/IMPL-Project-AIDerm/assets/21965720/02116bf3-159a-4c7b-817d-8c6441c1fa4f">


**Model Architecture:** 
The model architecture consists of two convolutional layers followed by max-pooling layers for feature extraction. The extracted features are then passed through two fully connected layers for classification.

<img width="321" alt="arch" src="https://github.com/aashimarora/IMPL-Project-AIDerm/assets/21965720/b49fe7a8-20e0-46e1-90e2-2c240e4ffe48">


## Performance
Accuracy of the network on the 895 test images: 54 %

Accuracy of Acne and Rosacea Photos : 90 %
Accuracy of Warts Molluscum and other Viral Infections : 37 %
Accuracy of Tinea Ringworm Candidiasis and other Fungal Infections : 28 %
Accuracy of Actinic Keratosis Basal Cell Carcinoma and other Malignant Lesions : 28 %
Accuracy of Seborrheic Keratoses and other Benign Tumors : 25 %
Accuracy of Systemic Disease : 14 %
Accuracy of Light Diseases and Disorders of Pigmentation : 13 %
Accuracy of Psoriasis pictures Lichen Planus and related diseases : 12 %
Accuracy of Lupus and other Connective Tissue diseases : 12 %
Accuracy of Atopic Dermatitis Photos :  8 %
Accuracy of Vascular Tumors :  8 %
Accuracy of Poison Ivy Photos and other Contact Dermatitis :  7 %
Accuracy of Urticaria Hives :  0 %
Accuracy of Eczema Photos :  0 %
Accuracy of Exanthems and Drug Eruptions :  0 %
Accuracy of Melanoma Skin Cancer Nevi and Moles :  0 %
Accuracy of Vasculitis Photos :  0 %
Accuracy of Cellulitis Impetigo and other Bacterial Infections :  0 %
Accuracy of Herpes HPV and other STDs Photos :  0 %


## Limitations

Limited Dataset: The model's performance may be limited by the size and diversity of the dataset. The 20 skin diseases dataset may not fully represent the variability of real-world skin conditions, leading to potential biases or generalization issues.
Computational Resources: Training and inference of the model require significant computational resources due to the model's architecture and the size of the input images. Deployment in resource-constrained environments may pose challenges.
Interpretability: The model's decision-making process may lack interpretability, hindering its adoption in clinical practice. Understanding the rationale behind the model's predictions is crucial for healthcare professionals but may be challenging with complex deep learning models.

## Trade-offs

Outline any trade-offs of your model, such as any circumstances where the model exhibits performance issues. 
Model Complexity vs. Computational Efficiency: The model's architecture strikes a balance between complexity and computational efficiency. While the model performs well in classifying skin lesions, it requires substantial resources for training and inference. Optimization efforts may be needed to improve efficiency without compromising performance.
Overfitting: The model architecture includes pooling layers to prevent overfitting. However, fine-tuning these hyperparameters may be necessary to achieve optimal performance across different datasets and environments. Balancing model regularization with capturing complex patterns is essential for robust performance.
