This project focuses on predicting motor coordination risk associated with Dyspraxia (Developmental Coordination Disorder – DCD) using deep learning based handwriting image analysis. Dyspraxia affects fine motor skills, handwriting, and coordination in children, making early detection essential for timely intervention. The proposed system uses EfficientNetB0 with transfer learning to extract discriminative handwriting features from 224×224 RGB images and classifies them into High Motor Coordination Risk or Mild Motor Coordination Risk. The model architecture consists of a pre-trained EfficientNetB0 backbone followed by Global Average Pooling, a 128-unit ReLU dense layer, dropout for regularization, and a Softmax output layer, enabling efficient, scalable, and accurate screening for dyspraxia-related motor difficulties.



 Training Results (Initial Fine-Tuned Model)

- Model: EfficientNetB0 (ImageNet pretrained)
- Fine-tuning: Last layers unfrozen
- Optimizer: Adam (low learning rate)
- Best Validation Accuracy: ~65%
- Observation: Validation accuracy improves after fine-tuning, indicating better feature adaptation for handwriting-based motor coordination patterns.

> Further improvements are planned using stronger data augmentation, class balancing, and extended fine-tuning.
