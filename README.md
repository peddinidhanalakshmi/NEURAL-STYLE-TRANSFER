# NEURAL-STYLE-TRANSFER
COMPANY : CODTECH IT SOLUTIONS

NAME : Peddini Dhana Lakshmi

INTERN ID : CT06DY2357

DOMAIN : Artificial Intelligence

DURATION : 6 WEEKS

# Description

Neural Style Transfer (NST) is an advanced technique in the field of Deep Learning and Computer Vision that allows us to blend the content of one image with the style of another image.

In simple terms, it enables the creation of artistic images by combining:

A content image (e.g., a photograph)

A style image (e.g., a painting)


The result is a new image that retains the content of the first image but adopts the artistic style (colors, textures, brush strokes) of the second image.

NST uses Convolutional Neural Networks (CNNs) — particularly pre-trained networks like VGG19 — to extract and manipulate features from both content and style images.
This process demonstrates how deep learning models can understand and recreate visual aesthetics.

Applications:

Creating AI-generated art

Enhancing photographs with artistic filters

Creative design and visual effects

#  Model Implementation Steps

The theoretical workflow of Neural Style Transfer can be described as follows:

Step 1: Importing Libraries

The model uses libraries such as TensorFlow, PyTorch, Keras, and OpenCV to handle image processing and deep learning operations.

Step 2: Loading Images

Two images are provided as inputs:

Content Image: The main image whose structure or layout will be preserved.

Style Image: The image whose color patterns and artistic effects will be applied.


Both images are resized and preprocessed to match the network’s input requirements.

Step 3: Using a Pre-trained CNN Model

A pre-trained deep learning model like VGG19 (trained on ImageNet dataset) is used for feature extraction.
This network contains multiple layers, each capable of recognizing different image features:

Lower layers: capture edges and textures.

Higher layers: capture complex shapes and styles.


Step 4: Extracting Features

Content features are extracted from the deeper layers (which focus on structure).

Style features are extracted from multiple layers (which focus on textures and colors).


Step 5: Defining Loss Functions

The NST algorithm optimizes a new image (called the generated image) by minimizing two main types of losses:

1. Content Loss: Measures the difference between the content of the generated image and the original content image.


2. Style Loss: Measures how different the textures and colors are between the generated image and the style image.

A total variation loss may also be added to improve smoothness.

Step 6: Optimizing the Image

An optimization algorithm (like Gradient Descent or Adam Optimizer) is used to iteratively adjust the generated image’s pixels to minimize the total loss.
Over multiple iterations, the image starts to resemble the content image but with the artistic patterns of the style image.

Step 7: Output the Styled Image

Once optimization is complete, the final image is de-normalized and displayed — showing the artistic transformation.

# Results

After implementing the Neural Style Transfer model, the system successfully creates a new image that:

Preserves the structure and content of the original (content) image.

Reflects the artistic style (colors, textures, brush strokes) of the style image.


The result demonstrates the capability of neural networks to understand and combine complex visual features from multiple sources.

For example:

Content Image: A photograph of a cityscape

Style Image: A painting by Van Gogh

Result: A cityscape that looks like it was painted in Van Gogh’s style.

# Output 
<img width="526" height="513" alt="Image" src="https://github.com/user-attachments/assets/5065f494-70bc-4a5e-83c8-f96e706f01cf" />

<img width="521" height="509" alt="Image" src="https://github.com/user-attachments/assets/b1dce9d6-f764-4dbf-ac4a-1b6876ebdc3c" />

