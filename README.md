🖼️ Stable Diffusion Image Generator
This project allows you to generate high-quality images from text prompts using Hugging Face's diffusers library and various pre-trained Stable Diffusion models.

📦 Features
Support for multiple Stable Diffusion models via a dictionary.

Easy-to-use CLI input with default parameters.

Automatic device selection (GPU if available).

Saves generated images with timestamped filenames.

Visualizes results using Matplotlib.

Resource cleanup to manage memory (especially on GPU).

🔧 Requirements
Install the required Python packages:

bash
Copy
Edit
pip install diffusers transformers accelerate torch pillow tqdm
🔐 Authentication
You must log in with your Hugging Face token to access the models:

python
Copy
Edit
from huggingface_hub import notebook_login
notebook_login()
🛠️ Usage
Run the script:

bash
Copy
Edit
python script_name.py
You will be prompted to enter image generation parameters such as:

Text prompt

Negative prompt

Number of inference steps

Guidance scale

Image dimensions

If no input is provided, default values will be used.

📁 Output
Generated images are saved in the generated_images directory with filenames that include the model name and timestamp.

🧠 Models
You can add more models to the MODEL_DICT dictionary in the script. Currently, it supports:

SG161222/Realistic_Vision_V3.0
