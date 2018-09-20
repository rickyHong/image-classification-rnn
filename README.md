### Project: Build an Image Classifier with RNN(LSTM) on Tensorflow

### next_batch : https://stackoverflow.com/questions/45110098/tensorflow-next-batch-function-of-np-array/45110647?noredirect=1#comment77193477_45110647

## https://www.researchgate.net/post/How_to_create_MNIST_type_database_from_images

## Models : https://www.tensorflow.org/api_docs/python/tf/contrib/rnn/BasicLSTMCell

### Highlights:

 - This is a **multi-class image classification** problem.
 - The purpose of this project is to **classify MNIST image dataset into 10 classes**. 
 - The model was built with **Recurrent Neural Network (RNN: LSTM)** on **Tensorflow**.
 
### Data:

  - The MNIST image dataset was saved in the ./data/ directory.

### Train:

 - Command: python3 train.py parameters.json
 - Example: ```python3 train.py ./parameters.json```
 
 A directory will be created during training, and the model will be saved in this directory. 

### Predict:

 Provide the model directory (created when running ```train.py```) to ```predict.py```.
 - Command: python3 predict.py ./trained_model_directory/
 - Example: ```python3 predict.py ./trained_model_1481170507/```

### Reference:
 - [Recurrent Neural Network](https://github.com/aymericdamien/TensorFlow-Examples/blob/master/examples/3_NeuralNetworks/recurrent_network.py)
 
 ### Cuda purge

dpkg -l | grep cuda- | awk '{print $2}' | xargs -n1 sudo dpkg --purge
dpkg --install cuda-repo-ubuntu*-8.0-local*.deb
sudo apt-get update
sudo apt-get install cuda
