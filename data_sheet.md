# Datasheet for the 20 Skin Diseases Dataset

## Motivation

- Purpose: The dataset was created to support research and development in dermatology, particularly in the domain of automated skin disease diagnosis using machine learning and computer vision techniques.
- Creator: The dataset was compiled and curated by Haroon Alam, an independent researcher, with the aim of advancing the understanding and diagnosis of various skin lesions and conditions.
- Funding: The creation of the dataset was self-funded by the author, Haroon Alam, as part of their independent research efforts.

## Composition

- Representation: The dataset comprises images of skin lesions and conditions representing 20 different dermatological diseases. These diseases include but are not limited to melanoma, psoriasis, eczema, acne, and others.
    Acne
    Actinic Carcinoma
    Atopic Dermatitis
    Bullous Disease
    Cellulitis
    Eczema
    Drug Eruptions
    Herpes HPV
    Light Diseases
    Lupus
    Melanoma
    Poison IVY
    Psoriasis
    Benign Tumors
    Systemic Disease
    Ringworm
    Urticarial Hives
    Vascular Tumors
    Vasculitis
    Viral Infections
    (Source: https://www.kaggle.com/datasets/haroonalam16/20-skin-diseases-dataset)

- Dataset Size: 
  - Length of Training Data: 2609 images
  - Length of Test Data: 895 images
- Missing Data: There is no missing data in the dataset.
- Confidentiality: The dataset does not contain any confidential information, as the images are anonymized and do not include any personally identifiable information.

## Collection Process

- Data Acquisition: The data collection process involved sourcing images from publicly available datasets and repositories, possibly including Kaggle. However, the exact sources and acquisition methods are unspecified.
- Sampling Strategy: The dataset represents a sample of skin lesion images collected from various sources. The sampling strategy, including selection criteria and representation balance, is not explicitly specified.
- Time Frame: The time frame for data collection is not provided, but it likely spanned several months to gather a diverse set of images representing different skin conditions.

## Preprocessing/Cleaning/Labeling

- Preprocessing:
  - Removed a Class: One class was removed from the test set as it did not have a corresponding class in the training set, ensuring consistency between the datasets.
  - Image Transformation: Images were resized to a standardized 192x192 resolution to facilitate compatibility with convolutional neural network (CNN) architectures.
  - Normalization: Image pixel values were normalized to a common scale to enhance model convergence and performance.
  - No Grayscaling: Grayscaling (converting images to grayscale) was not applied, preserving color information in the images as this is very important for conditions like Rosacea which indicates redness on the face or cystic acne including white materials.
- Raw Data: Both the raw and preprocessed versions of the data were saved to support potential future analyses and model improvements.

## Uses

- Other Tasks: In addition to automated skin disease diagnosis, the dataset could be utilized for tasks such as image classification, feature extraction, and anomaly detection in the field of computer vision.
- Considerations:
  - Use with Caution: Dataset consumers should exercise caution when interpreting the results of models trained on the dataset, as the dataset's composition and preprocessing steps may impact the generalizability of the models.
  - Medical Advice: The dataset should not be used as a standalone tool for providing dermatological advice or making treatment decisions. It should only complement the expertise of dermatologists and medical professionals.
- Restrictions: The dataset should not be used to make diagnostic or treatment decisions in clinical settings without proper validation and clinical supervision. Additionally, it should not be used to stigmatize or discriminate against individuals based on their skin conditions.

## Distribution

- Distribution: The distribution channels of the dataset are unknown. However, it may have been shared through platforms like Kaggle or research repositories.
- Copyright/IP License: The dataset's copyright status and intellectual property license are unspecified. Users should verify the applicable terms of use before accessing or utilizing the dataset.

## Maintenance

- Maintainer: The dataset is maintained by the author, Haroon Alam, who is responsible for updates, revisions, and addressing inquiries related to the dataset.