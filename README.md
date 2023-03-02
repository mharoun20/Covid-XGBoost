# Covid-XGBoost executive summary
- I aimed to diagnose COVID-19 using CT scans through the application of machine learning techniques.
- I started by downloading a dataset of CT scans from GitHub, which contained CT scans from both COVID-19 positive and negative patients.
- Images were preprocessed by resizing them and extracting features using a pre-trained ResNet50 model. The ResNet50 architecture was chosen for its high accuracy in image recognition tasks and its ability to handle the large size of the CT scans
- Extracted features were then fed into an XGBoost model, a powerful gradient boosting algorithm that has shown excellent performance in a wide range of classification tasks.
- I trained the model on 80% of the data, with a validation set comprising 10% and test set of 10% of the data.
- I evaluated the model on the unseen test set, which yielded a high AUC-ROC score of 0.83.
- One potential shortcoming of the model is the lack of interpretability. As it is a complex ensemble model, it is difficult to understand which features were most important for the model to make a decision.
- Future improvements could include the use of more advanced techniques for interpretability such as SHAP values, and the application of more advanced image processing techniques for feature extraction.
<img width="660" alt="Screen Shot 2023-03-01 at 10 30 28 PM" src="https://user-images.githubusercontent.com/87498313/222324014-c0cb4825-223b-4b13-bc9b-8c5b46858461.png">
