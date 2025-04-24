This project introduces NumPy for pixel-level image manipulation and TensorFlow for building a neural network to classify handwritten digits from the MNIST dataset. It is designed to help users understand NumPy array operations, which are foundational for working with machine learning frameworks like TensorFlow or PyTorch.

Purpose
NumPy Image Manipulation: Generate grayscale images (e.g., circles, radial waves, and mathematical patterns) using NumPy arrays and mathematical functions, visualized with Matplotlib.
TensorFlow MNIST Model: Train a basic neural network to classify MNIST digits, demonstrating TensorFlow's Keras API, model training, and prediction.

Prerequisites
Python 3.x
Required libraries:
numpy
matplotlib
tensorflow

Install dependencies:

bash
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
python script.py
Outputs: Grayscale images displayed/saved, MNIST training metrics, and prediction probabilities.
Google Colab:
Run the TensorFlow section in Colab: TensorFlow Quickstart.
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
