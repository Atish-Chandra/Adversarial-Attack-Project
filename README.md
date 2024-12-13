# Adversarial-Attack-Project
This project demonstrated how even high-performing models can be vulnerable to small, imperceptible perturbations, emphasizing the need for building more robust AI systems.
This project explores the robustness of deep learning models against adversarial perturbations. I have trained a DenseNet161 model on the Stanford Dogs Dataset to classify 120 dog breeds accurately. Then to challenge the model, I have implemented the DeepFool attack, generating subtle adversarial examples that caused the classifier to mispredict. Accordingly after that, to improve resilience, I have applied adversarial training, retraining the model with these adversarial examples to enhance robustness. This project highlights the vulnerabilities of complex CNN architectures and underscores the importance of building secure and reliable AI systems.

STEPS:-
1. Data Preparation 
Used the Stanford Dogs Dataset for training and evaluation.
Simplified the classification task to 120 dog breeds to reduce complexity.
Performed data preprocessing: resizing images, normalization, and creating train-test splits.
2. Model Definition 
Choose DenseNet161, a complex and efficient CNN architecture, as the backbone for the classifier.
Loaded pretrained weights (e.g., ImageNet) to accelerate training.
Fine tuned the model on the Stanford Dogs Dataset to achieve high accuracy.
3. DeepFool Attack Implementation ⚠
Implemented the DeepFool attack, an adversarial attack that generates minimal perturbations to fool the model.
Generated adversarial examples by iteratively perturbing input images.
Visualization: Compared clean images and adversarial examples to observe subtle perturbations.
Analyzed how these small perturbations misled the model into incorrect predictions.
4. Evaluation of Model Robustness 
Evaluated the classifier’s performance on clean images and adversarial examples.
Observed significant drops in accuracy, highlighting the model's vulnerability to adversarial attacks.
5. Adversarial Training 
Retrained the model using a combination of clean and adversarial examples.
Integrated adversarial examples into the training process to improve robustness.
Compared model accuracy before and after adversarial training on both clean and adversarial inputs.
6. Post-Adversarial Training Analysis 
Reapplied the DeepFool attack to test the robustness of the retrained model.
Visualized improvements: the model showed better resilience to adversarial perturbations.
Evaluated final results to confirm improved robustness while maintaining performance on clean data.
