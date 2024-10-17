This project focuses on binary classification for motor vehicle insurance claims, where the goal is to classify each claim as either Fraud (1) or Non-fraud (0). The training dataset is highly imbalanced, with 6,091 non-fraud cases and only 372 fraud cases. To address this, I employed a combination of techniques to generate synthetic fraud images and create a more balanced dataset for training.

To overcome the data imbalance, traditional data augmentation methods were used alongside Generative Adversarial Networks (GANs), which were specifically employed to generate synthetic fraud images. Additionally, SMOTE (Synthetic Minority Oversampling Technique) was applied to further augment the fraud class by generating synthetic samples based on the existing ones. These methods prevent the model from becoming biased toward the majority class, improving its ability to accurately predict fraudulent claims.

Each of these balancing techniques was implemented in dedicated notebooks, named as follows:

	•	Traditional Data Augmentation: aug_cnn_model_refresh.ipynb
	•	SMOTE: smote_cnn_model_refresh.ipynb
	•	GAN: gan_cnn_model_refresh.ipynb
	•	Combination of Traditional Augmentation and GAN: cnn_model_refresh.ipynb

The dataset used for this project is publicly available on Kaggle: Vehicle Insurance Fraud Classification. By applying these various balancing techniques, the model was trained on a more equitable representation of both fraud and non-fraud cases, mitigating the risk of overfitting to the majority class.

Addressing data imbalance is crucial in fraud detection tasks, as it helps the model generalize better and make accurate predictions on both minority and majority classes. The combination of traditional augmentation, GAN, and SMOTE resulted in a robust model capable of detecting fraudulent claims more effectively.
