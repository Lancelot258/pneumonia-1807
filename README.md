
This is a try-out project, which used to help me study ML&AI. 
For personal usage and hope this can benefit u!

# Pneumonia Detection Web Application

This project is a Flask-based web application for detecting pneumonia from uploaded chest X-ray images using a pre-trained deep learning model.

---

## Project Structure

```
Pneumonia-Detection-WebApp/
|-- Pneumonia/                # Contains the pre-trained model files
|   |-- variables/            # Model variable files
|       |-- variables.data-00000-of-00001
|       |-- variables.index
|   |-- keras_metadata.pb     # Metadata for the Keras model
|   |-- saved_model.pb        # Saved model file
|
|-- static/                   # Static assets folder (e.g., test files)
|   |-- test.txt
|
|-- templates/                # HTML templates for rendering the web pages
|   |-- index.html            # Main HTML template
|
|-- app.py                    # Main application logic for Flask
|-- requirements.txt          # Python dependencies for the project
|-- Procfile                  # Deployment configuration for Heroku
|-- README.md                 # Project documentation (this file)
```

---

## Features

1. **Image Upload**: Users can upload chest X-ray images through the web interface.
2. **Deep Learning Model**: The uploaded images are processed using a pre-trained pneumonia detection model.
3. **Prediction Display**: The application returns the prediction results on the web page.

---

## Requirements

### Software Requirements:
- Python 3.8 or above
- Flask framework

### Libraries:
Refer to `requirements.txt` for the complete list of dependencies:

```
absl-py==1.0.0
astunparse==1.6.3
cachetools==5.0.0
certifi==2021.10.8
charset-normalizer==2.0.11
click==8.0.3
colorama==0.4.4
Flask==2.0.2
flatbuffers==2.0
gast==0.5.3
google-auth==2.6.0
google-auth-oauthlib==0.4.6
google-pasta==0.2.0
grpcio==1.43.0
gunicorn==20.1.0
h5py==3.6.0
idna==3.3
importlib-metadata==4.10.1
itsdangerous==2.0.1
Jinja2==3.0.3
joblib==1.1.0
keras==2.8.0
Keras-Preprocessing==1.1.2
libclang==13.0.0
Markdown==3.3.6
MarkupSafe==2.0.1
numpy==1.22.2
oauthlib==3.2.0
opt-einsum==3.3.0
protobuf==3.19.4
pyasn1==0.4.8
pyasn1-modules==0.2.8
requests==2.27.1
requests-oauthlib==1.3.1
rsa==4.8
scikit-learn==1.0.2
scipy==1.8.0
six==1.16.0
sklearn==0.0
tensorboard==2.8.0
tensorboard-data-server==0.6.1
tensorboard-plugin-wit==1.8.1
tensorflow-cpu
tensorflow-io-gcs-filesystem==0.24.0
termcolor==1.1.0
tf-estimator-nightly==2.8.0.dev2021122109
threadpoolctl==3.1.0
typing_extensions==4.0.1
urllib3==1.26.8
Werkzeug==2.0.3
wrapt==1.13.3
zipp==3.7.0
pillow==9.0
```

---

## Installation and Setup

### Step 1: Clone the Repository
```bash
git clone <repository_url>
cd Pneumonia-Detection-WebApp
```

### Step 2: Create a Virtual Environment
```bash
python3 -m venv env
source env/bin/activate   # On Linux/Mac
env\Scripts\activate    # On Windows
```

### Step 3: Install Dependencies
```bash
pip install -r requirements.txt
```

### Step 4: Run the Application
```bash
python app.py
```

The application will run locally at `http://127.0.0.1:5000/`.

---

## Deployment (Heroku)

### Step 1: Install Heroku CLI
Refer to [Heroku CLI Installation Guide](https://devcenter.heroku.com/articles/heroku-cli).

### Step 2: Create a Heroku Application
```bash
heroku create <app_name>
```

### Step 3: Deploy the Application
```bash
git add .
git commit -m "Initial commit"
git push heroku main
```

### Step 4: Open the Deployed App
```bash
heroku open
```

---

## Notes

- Ensure that the `Pneumonia` folder contains the trained model files (`saved_model.pb` and variable files).
- Test images can be placed in the `static` folder for quick testing.
- Update the Flask `app.py` if new routes or functionalities are added.

---

## License
This project is licensed under the MIT License. See the `LICENSE` file for more details.

---

## Author
**Lancelot**
- Email: lancelottyy38@gmail.com



