Style Transfer Using Convolutional Neural Networks
This repository demonstrates image style transfer using convolutional neural networks (CNNs), based on the technique described by Gatys et al. in "Image Style Transfer Using Convolutional Neural Networks". The project uses the VGG19 model to blend the content of one image with the style of another, creating unique and visually striking results.

Project Overview
The style transfer process involves combining the content of a target image with the style of a reference image. This is achieved through the following steps:

Preprocessing: Load and preprocess images to fit the input shape of the model.
Feature Extraction: Use the VGG19 model to extract content and style features.
Gram Matrix Calculation: Compute the Gram matrix to capture style information.
Loss Computation: Calculate content and style losses to guide the optimization process.
Optimization: Update the target image to minimize the total loss, balancing content preservation and style application.
Features
Content Loss: Measures the difference between the content of the target image and the content of the original image.
Style Loss: Measures the difference between the style of the target image and the style of the reference image, using the Gram matrix for style representations.
Optimized Target Image: Iteratively updated to achieve a blend of the content and style images.
Setup
Clone the Repository:

bash
Copy code
git clone https://github.com/your-username/style-transfer-project.git
Install Dependencies:
Make sure you have the required Python libraries installed. You can use the provided requirements.txt file to install dependencies:

bash
Copy code
pip install -r requirements.txt
Run the Jupyter Notebook:
Open the Jupyter notebook included in the repository to execute the style transfer process:

bash
Copy code
jupyter notebook
Navigate to style_transfer.ipynb and follow the instructions in the notebook.

Usage
Load Content and Style Images:
Update the paths or URLs in the notebook to load your own content and style images.

Adjust Parameters:
Modify the content and style weights to control the balance between content preservation and style application.

Execute Style Transfer:
Run the notebook cells to perform style transfer and view the resulting images.

Example
Here's an example of a style transfer result:
![image](https://github.com/user-attachments/assets/40cd7177-bcc3-4f66-9aa7-dee0170ad608)


License
This project is licensed under the MIT License. See the LICENSE file for details.

Acknowledgements
Gatys et al., "Image Style Transfer Using Convolutional Neural Networks"
VGG19 model and pretrained weights provided by PyTorch
