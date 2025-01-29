In this project, I have tried to make a model that can predict images of 5 cricket players from India - Virat Kohli, Rohit Sharma, Mohammad Shami, MS Dhoni and Sachin Tendulkar.
Out of SVM, RandomForest and Logistic Regression, SVM performed the best in my case so I have used that model to detect players in the website

The link to the dataset used to train this model is: https://drive.google.com/drive/folders/1eQsg9AH66i2y7TF2STUBoMqjAjI2umJ8?usp=drive_link
Feel free to add more images to the dataset as it can improve the score of the model.
The images for this project was downloaded from google by searching player name and using a chrome extension called "FAKTUN"

The following steps were involved in this project:

1. Data collection: done using Faktun chrome extension.
2. Data cleaning and preprocessing: in model folder, the jupyter notebook has all this steps. Only images in which the face and two eyes are completely visible are taken for model training.
   The original image and image after wavelet function were vertically stacked for model training.
3. Model training: creation of training and testing sets. Training data on 3 classification algorithms- SVM, RandomForest and Logistic Regression. The model with the best score is taken.
4. Flask Server creation: in Flask folder there are 3 files- Server.py, util.py and wavelet.py. Wavelet.py is for input image transformation, util.py for utility functions and Server.py is the actual server code.
5. Web UI creation.

To run this project on your machine: 
1. Run Server.py from Flask folder
2. Open app.html from UI folder
3. Input any image and get results

   UI of final product:

   ![image](https://github.com/user-attachments/assets/a106fa97-75f1-4bee-b2c5-c7cead00b4d9)


   NOTE: I have given path of datasets and images stored in my machine. DON'T forget to modify paths when running on your PC.

This project is made taking reference from the following project: https://github.com/codebasics/py/tree/master/DataScience/CelebrityFaceRecognition
