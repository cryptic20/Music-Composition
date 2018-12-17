# Music-Composition
Using RNN to generate a classical piece based on the [article](https://towardsdatascience.com/how-to-generate-music-using-a-lstm-neural-network-in-keras-68786834d4c5).

## Requirements
Python3.X
* Keras
* Music21
* Tensorflow
* h5py


## Data input for training ##
  Any set of MIDI files consisting of a single instrument would work for this model. 
  Store the midi files under the directory "midi_songs".


## Training ##
To begin training, run ```python lstm.py```
* note: make sure to specify the directory of the midi files that you want to train. E.g ```train_network('path_to_your_midi_files')```

## Generating Music ##
To generate a piece, input the proper model weights in *predict.py* ``` model.load_weights('weights.hdf5') ``` with the weights that have been created after training
and simply run ```python preditct.py```
