## PROJECT TITLE 

#### AI Dermatologist: Detect skin lesions in a multi-class classification problem using CNNs

### NON-TECHNICAL EXPLANATION OF YOUR PROJECT
An AI dermatologist utilizing a skin diseases dataset employs Convolutional Neural Networks (CNNs) to analyze dermatological images. Through deep learning, CNNs automatically extract features from images, aiding in the classification of various skin conditions such as melanoma, psoriasis, and eczema. Trained on a diverse dataset, the model learns to distinguish between different skin diseases, assisting dermatologists in accurate diagnosis and treatment planning. This technology revolutionizes dermatology by providing efficient and reliable support in image-based diagnosis, enhancing patient care and outcomes through the integration of artificial intelligence in clinical practice.

### DATA
I am using the 20 Skin diseases dataset.

https://www.kaggle.com/datasets/haroonalam16/20-skin-diseases-dataset

('Acne and Rosacea Photos', 840), ('Actinic Keratosis Basal Cell Carcinoma and other Malignant Lesions', 322), ('Light Diseases and Disorders of Pigmentation', 299), ('Warts Molluscum and other Viral Infections', 248), ('Tinea Ringworm Candidiasis and other Fungal Infections', 122), ('Vascular Tumors', 101), ('Atopic Dermatitis Photos', 100), ('Lupus and other Connective Tissue diseases', 90), ('Systemic Disease', 81), ('Seborrheic Keratoses and other Benign Tumors', 80), ('Cellulitis Impetigo and other Bacterial Infections', 65), ('Poison Ivy Photos and other Contact Dermatitis', 62), ('Psoriasis pictures Lichen Planus and related diseases', 62), ('Herpes HPV and other STDs Photos', 40), ('Eczema Photos', 35), ('Melanoma Skin Cancer Nevi and Moles', 24), ('Exanthems and Drug Eruptions', 20), ('Vasculitis Photos', 15), ('Urticaria Hives', 3)

### MODEL 
I am using a CNN architecture inspired my LeNet5. CNNs offer a powerful and versatile framework for image analysis in dermatology, enabling automated diagnosis, classification, and decision support in clinical practice. Their ability to learn discriminative features directly from raw images makes them indispensable tools for AI-driven dermatological diagnosis and patient care.

#### HYPERPARAMETER OPTIMISATION
Various hyperparamters that I chose to tune were:
Learning Rate, Optimizer, number of epochs, Additonal CNN layers, number of filters, size of kernel, add dropout to prevent overfitting.

I used the following ideas: 
Learning Rate: Ensure that the learning rate used for training is appropriate. If the learning rate is too high, the optimization process may overshoot the optimal solution and fail to converge. Conversely, if the learning rate is too low, the optimization process may progress very slowly. Experiment with adjusting the learning rate, either increasing or decreasing it, and observe its impact on the loss curve.

Inspect Model Complexity: Evaluate if the model architecture is sufficiently complex to capture the underlying patterns in the data. If the model is too simple, it may struggle to learn the intricacies of the dataset, leading to poor performance. Consider increasing the model's capacity by adding more layers, increasing the number of filters in convolutional layers, or adding dropout layers to prevent overfitting.

Check Data Preprocessing: Ensure that the input data is preprocessed appropriately. Common preprocessing steps include normalization (scaling pixel values to the range [0, 1] or [-1, 1]), data augmentation (randomly applying transformations such as rotation, flipping, or scaling to increase dataset diversity), and handling missing or noisy data.

Increase Training Epochs: Sometimes, the model may require more training epochs to converge to a good solution. Try increasing the number of epochs beyond 5 and monitor the loss curve. However, be cautious of overfitting if training for too many epochs without regularization techniques.

Monitor Validation Loss: Check if the validation loss is also stagnant or increasing. If the validation loss is increasing while the training loss remains constant, it indicates overfitting. In such cases, consider using techniques like early stopping or regularization (e.g., dropout, weight decay) to prevent overfitting.

Explore Different Optimizers: Experiment with different optimization algorithms such as Adam, RMSprop, or SGD with momentum. Each optimizer has its strengths and may perform differently on your specific problem and dataset.

Debug Model Implementation: Double-check the implementation of your CNN model, loss function, and data loading pipeline for any bugs or inconsistencies. Ensure that the forward pass, backward pass, and gradient updates are correctly implemented.

### RESULTS
The dataset is imbalanced and produced the following results on each of the classes. The overall accuracy was 54 % 
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