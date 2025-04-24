This project demonstrates basic image manipulation using NumPy and a neural network for MNIST digit classification using TensorFlow. It serves as an introduction to NumPy for image processing and TensorFlow for machine learning.

Purpose
NumPy: Generate grayscale images (e.g., circles, radial waves, patterns) using mathematical functions and array operations.
TensorFlow: Train a simple neural network to classify handwritten digits from the MNIST dataset.
Prerequisites
Python 3.x
Required libraries:
numpy
matplotlib
tensorflow
Install dependencies:

bash

Copy
pip install numpy matplotlib tensorflow
Project Structure
NumPy Image Manipulation:
Creates 240x320 or 256x256 grayscale images using NumPy arrays.
Examples include:
Random 10x10 pixel images.
Circles (parametric and distance-based methods).
Radial waves, spirals, and other patterns using sin, cos, and exp.
Visualizes images with Matplotlib and saves them as PNGs (e.g., custom_image.png, radial_wave_image.png).
TensorFlow MNIST Model:
Loads and normalizes the MNIST dataset.
Defines a Keras sequential model:
Flatten layer (28x28 input).
Dense layer (128 units, ReLU).
Dropout (20%).
Dense output layer (10 units).
Compiles with Adam optimizer and sparse categorical crossentropy loss.
Trains for 5 epochs and outputs softmax probabilities for test samples.
How to Run
Local Execution:
Clone the repository or save the script as script.py.
Run the script:
bash

Copy
python script.py
Outputs: Grayscale images displayed/saved, MNIST training metrics, and prediction probabilities.
Google Colab:
Run the TensorFlow section in Colab: TensorFlow Quickstart.
Example Outputs
NumPy Images:
Grayscale patterns (e.g., circles, radial waves) displayed and saved.
TensorFlow Training:
text
Examples

Epoch 1/5
1/1 [==============================] - 0s 40ms/step - accuracy: 1.0000 - loss: 0.0141
...
Epoch 5/5
1/1 [==============================] - 0s 41ms/step - accuracy: 1.0000 - loss: 0.0013
Loss: 0.014134535565972328, Accuracy: 1.0

tf.Tensor(
[[9.0462407e-03 3.8271805e-03 3.7947576e-03 9.6926528e-01 1.4459594e-03
  4.4702939e-03 1.8479681e-03 2.2493138e-03 3.2946530e-03 7.5842155e-04]
 [3.6800732e-03 3.2825512e-03 2.1717104e-03 9.8108619e-01 1.6960469e-03
  2.4490596e-03 7.1367127e-04 2.0476931e-03 2.6178844e-03 2.5512266e-04]
