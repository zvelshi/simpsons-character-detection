## 🍩 Simpsons Character Detection
This project a deep learning model to recognize characters from the TV show "The Simpsons" using images. It follows these major steps:
1. Data Preprocessing: It reads images representing character images from a given dataset, then creates a dictionary to store the count of images for each character and sorts it in descending order.
2. Selecting Characters: The top 10 characters with the most images are selected and stored in a list.
3. Creating Training Data: Images of the selected characters are preprocessed and loaded as training data, considering the specified image size and channel count. The data is shuffled for training.
4. Data Normalization and Label Conversion: The data is normalized to the range (0,1) and the numerical labels are converted into binary class vectors using one-hot encoding.
5. Train-Validation Split: The training data is split into training and validation sets using the specified validation ratio.
6. Model Creation: A convolutional neural network model is created with specified parameters like image size, channel count, output dimension, loss function, learning rate, etc. The model summary is displayed.
7. Model Training: The model is trained using the training generator with specified batch size and epochs. A learning rate scheduler callback is applied during training.
8. Testing: A sample test image of a character ("Charles Montgomery Burns") is loaded and prepared. The trained model predicts the character in the image, and the character with the highest predicted probability is printed.

## 🔨 Key Technologies Used
* OpenCV
* TensorFlow
* Python: NumPy

## Program In Action
<img src="simps_data/characters_illustration.png? raw=true"/>
<img src="images/cmd.JPG? raw=true"/>
<img src="images/burns.png? raw=true"/>
