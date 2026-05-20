# Laboratory-Work-5-Activity-Comparative-Analysis

# Google Collab

[CLICK HERE TO VIEW THE COLLAB](https://colab.research.google.com/drive/1QNOFl2ElBaFMG0AXBLhDfFOre6G-8Fxb?usp=sharing).

# New Keras Model

[CLICK HERE TO VIEW THE COLLAB](https://drive.google.com/file/d/1AVMQNw_ZyCZDHrHzTlA1NTRgDjJfTNyE/view?usp=drive_link).



Performance Comparison Table

<img width="529" height="478" alt="image" src="https://github.com/user-attachments/assets/949f2f68-7c80-4a35-acc6-2bf8859d4b26" />


A. Model Performance

1. Which pre-trained model achieved the highest accuracy? Why?

VGG16 achieved the highest accuracy among all the tested models. It was able to extract image features more effectively and produced more stable predictions during validation. The architecture of VGG16 worked well with the dataset used in this project. Its simpler and deeper layer structure helped improve classification performance.

2. Which model had the lowest performance? What could be the reason?

EfficientNetB3 showed the lowest performance in the experiment. One possible reason is that the model may require more training time and better parameter tuning. The dataset may also not have been large enough for the model to learn effectively. Another factor could be overfitting or insufficient feature extraction during training.

3. How did loss values compare across models?

VGG16 had the lowest training and validation loss values compared to the other models. Lower loss means the model made fewer prediction errors during training and testing. EfficientNetB3 and ResNet101 had higher loss values, showing weaker performance. The loss values helped confirm which model learned the dataset more effectively.

B. Evaluation Metrics

4. Why is accuracy not enough to evaluate a model?

Accuracy alone does not always reflect the true performance of a model. A model can have high accuracy but still perform poorly on certain classes. Metrics such as precision, recall, and F1-score provide a deeper understanding of prediction quality. These metrics are especially important when dealing with class imbalance or misclassifications.

5. Which model had the best F1-score? What does it indicate?

VGG16 achieved the best F1-score among the tested models. The F1-score measures the balance between precision and recall. A high F1-score means the model performs well in both correctly predicting classes and minimizing errors. This indicates that VGG16 produced more reliable and balanced predictions.

6. How did Precision and Recall differ across models?

VGG16 showed higher precision and recall values than the other models. This means it correctly identified more images while also reducing incorrect predictions. EfficientNetB3 and ResNet101 struggled more in distinguishing similar classes. The differences in precision and recall highlighted the strengths and weaknesses of each model.

C. Confusion Matrix Analysis

7. Which classes were frequently misclassified?

Classes with similar visual appearances were more frequently misclassified by the models. Some images may have contained overlapping features or unclear patterns. This caused the models to confuse one class with another during prediction. Misclassification was more noticeable in the weaker-performing models.

8. What patterns did you observe in the confusion matrix?

The confusion matrix showed that VGG16 produced more correct predictions along the diagonal line. This indicates better classification accuracy for most classes. Other models showed more scattered values outside the diagonal, meaning more prediction errors occurred. The matrix helped visualize which classes were hardest to classify.

D. ROC and AUC

9. Which model had the highest AUC score?

VGG16 achieved the highest AUC score among the tested models. A higher AUC means the model was better at separating different classes correctly. This indicates that VGG16 had stronger classification capability and more consistent predictions. The ROC curve also showed better performance compared to the other models.

10. What does AUC tell us about model performance?

AUC measures how well a model can distinguish between classes. A higher AUC score means the model has better prediction performance. It helps evaluate the classifier beyond simple accuracy values. Models with high AUC are generally more reliable in classification tasks.

E. Explainability (Grad-CAM)

11. What did Grad-CAM reveal about model decision-making?

Grad-CAM showed the important image regions used by the model during prediction. It highlighted which parts of the image influenced the classification result the most. This helped explain how the model made decisions internally. Grad-CAM also improved the interpretability of the CNN models.

12. Did the model focus on relevant image regions?

Yes, the better-performing models focused on relevant object regions instead of unnecessary background details. This showed that the model learned meaningful visual patterns from the dataset. Some weaker models focused on less important regions, which affected prediction quality. Proper attention to image features improved overall accuracy.

13. Which model produced the most meaningful heatmaps?

VGG16 produced the clearest and most meaningful Grad-CAM heatmaps. The highlighted regions closely matched the important parts of the objects in the images. This indicates that the model learned useful features during training. The heatmaps also showed why VGG16 achieved better performance.

F. Model Comparison & Improvement

14. Which model would you recommend for deployment? Why?

VGG16 is the most recommended model for deployment in this project. It achieved the best performance in terms of accuracy, loss, F1-score, and AUC score. The model also produced clearer Grad-CAM visualizations and more stable predictions. Its overall reliability makes it suitable for real-world applications.

15. How can you further improve your best-performing model?

The model can be improved by increasing the dataset size and adding more diverse images. Data augmentation techniques can also help improve generalization performance. Fine-tuning more layers and training for additional epochs may further increase accuracy. Hyperparameter tuning can also optimize the model’s learning process.

G. Real-World Application

16. How can your model be applied in real-world scenarios?

The model can be used in different image recognition applications such as medical diagnosis, security systems, and product classification. It can help automate tasks that involve identifying objects from images. Businesses and organizations can use it to improve efficiency and reduce manual work. CNN models are widely used in many AI-powered systems today.

17. What are the risks of deploying an inaccurate model?

An inaccurate model may produce incorrect predictions that can affect decision-making. In sensitive applications, such as healthcare or security, wrong predictions can lead to serious problems. Poor model performance may also reduce user trust and system reliability. Continuous testing and monitoring are important before deployment.

18. How can this system be integrated into a mobile/web app?

The trained CNN model can be integrated into a web or mobile application using frameworks like Flask or TensorFlow Lite. Users can upload images, and the system can instantly generate predictions. APIs can connect the trained model to the frontend interface for real-time processing. This allows the model to be accessible and usable in practical environments.
