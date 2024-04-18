# Model Card


## Model Description

**Input:** 
The input to the model is a 192x192 RGB image representing a skin lesion. Each image contains three channels corresponding to red, green, and blue color intensities.

**Output:** 
The output of the model is a probability distribution over the classes of skin lesions present in the input image. The model predicts the likelihood of each class, including but not limited to melanoma, psoriasis, eczema, and acne.

**Model Architecture:** 
The model architecture consists of two convolutional layers followed by max-pooling layers for feature extraction. The extracted features are then passed through two fully connected layers for classification.

## Performance
Accuracy of the network on the 895 test images: 53 %

Accuracy of Acne and Rosacea Photos : 94 %
Accuracy of Seborrheic Keratoses and other Benign Tumors : 22 %
Accuracy of Actinic Keratosis Basal Cell Carcinoma and other Malignant Lesions : 22 %
Accuracy of Tinea Ringworm Candidiasis and other Fungal Infections : 21 %
Accuracy of Herpes HPV and other STDs Photos : 16 %
Accuracy of Lupus and other Connective Tissue diseases : 16 %
Accuracy of Warts Molluscum and other Viral Infections : 15 %
Accuracy of Systemic Disease : 11 %
Accuracy of Poison Ivy Photos and other Contact Dermatitis :  7 %
Accuracy of Cellulitis Impetigo and other Bacterial Infections :  7 %
Accuracy of Vascular Tumors :  5 %
Accuracy of Psoriasis pictures Lichen Planus and related diseases :  4 %
Accuracy of Atopic Dermatitis Photos :  4 %
Accuracy of Light Diseases and Disorders of Pigmentation :  3 %
Accuracy of Urticaria Hives :  0 %
Accuracy of Eczema Photos :  0 %
Accuracy of Exanthems and Drug Eruptions :  0 %
Accuracy of Melanoma Skin Cancer Nevi and Moles :  0 %
Accuracy of Vasculitis Photos :  0 %

## Limitations

Limited Dataset: The model's performance may be limited by the size and diversity of the dataset. The 20 skin diseases dataset may not fully represent the variability of real-world skin conditions, leading to potential biases or generalization issues.
Computational Resources: Training and inference of the model require significant computational resources due to the model's architecture and the size of the input images. Deployment in resource-constrained environments may pose challenges.
Interpretability: The model's decision-making process may lack interpretability, hindering its adoption in clinical practice. Understanding the rationale behind the model's predictions is crucial for healthcare professionals but may be challenging with complex deep learning models.

## Trade-offs

Outline any trade-offs of your model, such as any circumstances where the model exhibits performance issues. 
Model Complexity vs. Computational Efficiency: The model's architecture strikes a balance between complexity and computational efficiency. While the model performs well in classifying skin lesions, it requires substantial resources for training and inference. Optimization efforts may be needed to improve efficiency without compromising performance.
Overfitting: The model architecture includes pooling layers to prevent overfitting. However, fine-tuning these hyperparameters may be necessary to achieve optimal performance across different datasets and environments. Balancing model regularization with capturing complex patterns is essential for robust performance.