# Style_Transfer_Project
This project implements an artistic style transfer algorithm using TensorFlow and the VGG19 model. The code transforms a given content image by applying the style of a separate style image, resulting in a new, stylized creation.


Key Components of the Code:

1.Importing Libraries: The script uses TensorFlow, NumPy, and Matplotlib for neural network operations, numerical computations, and image display.

2.Image Preprocessing Functions:

  preprocess_image: Loads and processes images to conform with VGG19 input requirements.
  deprocess_img: Reverts the preprocessing to display images in their original form.
3.Loading and Preprocessing Images:

  Content and style images are loaded and preprocessed using the defined functions.

4.VGG19 Model Configuration:

  The pre-trained VGG19 model is loaded and configured to output intermediate layers' activations, essential for style transfer.

5.Loss Functions:

  compute_style_loss and compute_content_loss: Calculate the style and content loss, respectively.
  gram_matrix: A helper function used in style loss calculation.

6.Total Loss Calculation:

   compute_loss: Calculates the total loss, combining style and content loss.

7. Optimization:

  train_step: Defines a single optimization step, adjusting the target image to minimize the total loss.
  An Adam optimizer is used for optimization in a training loop, progressively stylizing the content image.
