*Deep Fake Detection Django Application*
**System Requirements**

NVIDIA GPU (required)
CUDA version 10.0 or higher
GPU Compute Capability > 3.0
Python 3.6+
Django 3.0+

For a complete list of dependencies, refer to the requirements.txt file in the project root.

**Project Structure**

ml_app: Contains core application logic (views.py)
project_settings: Django configuration files
static: CSS, JavaScript, and JSON assets (including face-api files)
templates: HTML template files

Before running the application, create the following directories in the project root:

.../models/
.../uploaded_images/
.../uploaded_videos/

Ensure you have the necessary permissions to access these directories.
Local Setup and Deployment

##Clone the repository:##

Navigate to the Django application directory.

Create and activate a virtual environment(Optional):

python -m venv venv
venv\Scripts\activate

Install required packages:
pip install -r requirements.txt

Place your trained model in the models directory.
You can download our models from google drive [https://drive.google.com/drive/folders/1yDsQ3YFTTD0n9Efk6eyTJ2a_zq3_fYq1?usp=sharing]
The model filename should follow this format: model_[accuracy]_acc_[num_frames]_frames_final_data.pt
Example: model_84_acc_10_frames_final_data.pt (for a 10-frame model)

Start the Django development server:
python manage.py runserver


After completing these steps, the application should be running locally on your machine.
Note: This application requires significant computational resources. Ensure your system meets the hardware requirements before attempting to run it.
