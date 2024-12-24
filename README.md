# Image-classifier-model
An Image Classifier API using FastAPI and scikit-learn to classify images into categories. It preprocesses images (grayscale, resize, flatten), trains an SVM model, and provides a /predict/ endpoint to upload images and get predicted classes with confidence scores. Ideal for simple image categorization tasks.
..
.
.
The project structure can be summarized as follows:
text_classification/
├── app/
│   ├── main.py         # FastAPI app
│   ├── routes.py       # API routes
├── model/
│   ├── train.py        # Model training
│   ├── predict.py      # Prediction logic
├── requirements.txt    # Dependencies
└── README.md          # Documentation

.
.
.
.
To run the application:

Install dependencies: pip install -r requirements.txt
Train the model: python model/train.py
Run FastAPI: uvicorn app.main:app --reload
.
.
.
.


Steps to Upload the File in Postman:
Open Postman.
Set the request method to POST and the URL to http://127.0.0.1:8000/predict/.
Go to the Body tab.
Select form-data as the body type.
Add a key named file (case-sensitive and must match the FastAPI parameter name).
Select the File option from the dropdown menu next to the key.
Click the Choose File button and navigate to your file path (e.g., D:\image_classification\dataset\images\class1\image1.jpg) to upload the image.
