# Deep fake detection Django Application
## Requirements:

**Note :** Nvidia GPU is mandatory to run the application.
- CUDA version >= 10.0 for GPU
- GPU Compute Capability > 3.0 


You can find the list of requirements in the requirement.txt

```
Python >= v3.6
Django >= v3.0
```

## Directory Structure

- ml_app -> Directory containing code in views.py file
- project_settings -> Contains Django settings and files to run in production
- static -> Contains all css, js and json files (for face-api)
- templates -> Template files for HTML

<b>Note:</b> Before running the project make sure you have created directories namely <strong>models, uploaded_images, uploaded_videos</strong> in the project root and that you have proper permissions to access them.

# Running application locally on your machine

### Prerequisite
1. Copy your trained model to the models folder.
   

#### Step 1 : Clone the repo and Navigate to Django Application

`git clone https://github.com/https://github.com/Vishal-1024/AI-ML_Hackathon_Deepfake-detection.git`

#### Step 2: Create virtualenv (optional)

`python -m venv venv`

#### Step 3: Activate virtualenv (optional)

`venv\Scripts\activate`

#### Step 4: Install requirements

`pip install -r requirements.txt`

#### Step 5: Copy Models

`Copy your trained model to the models folder i.e Django Application/models/`

- You can download our trained models from our google drive [https://drive.google.com/drive/folders/1yDsQ3YFTTD0n9Efk6eyTJ2a_zq3_fYq1?usp=sharing]

**Note :** The model name must be in specified format only i.e *model_84_acc_10_frames_final_data.pt*. Make sure that no of frames must be mentioned after certain 3 underscores `_` , in the above example the model is for 10 frames.


### Step 6: Run project

`python manage.py runserver`

 
