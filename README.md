# How-to-Generate-Music-Demo
This is the code for "How to Generate Music - Intro to Deep Learning #9' by Siraj Raval on YouTube

##Overview

This is the code for [this]() video on Youtube by Siraj Raval as part of the the Udacity Deep Learning Nanodegree. It uses Keras & Theano, two deep learning libraries, to generate jazz music. Specifically, it builds a two-layer LSTM, learning from the given MIDI file. 

##Dependencies

* [Keras](http://keras.io/#installation)
* [Theano](http://deeplearning.net/software/theano/install.html#bleeding-edge-install-instructions) ("bleeding-edge" version on GitHub)
* [music21](http://web.mit.edu/music21/doc/installing/index.html)

##Usage

Run on CPU with command:  
```
python generator.py [# of epochs]
```

Run on GPU with command:  
```
THEANO_FLAGS=mode=FAST_RUN,device=gpu,floatX=float32 python generator.py [# of epochs]
```
Note: running Keras/Theano on GPU is formally supported for only NVIDIA cards (CUDA backend).

Note: `preprocess.py` must be modified to work with other MIDI files (the relevant "melody" MIDI part needs to be selected). 

#Coding Challenge - Due Date is Thursday, March 16th 2017 at 12 PM PST

The challenge is to generate your own MIDI file! This code trains off of a single MIDI file and the preprocess.py file manually selects the relevant melody part. Modify it so that it selects the melody from your own MIDI file. Bonus points if you train it on not one, but multiple MIDI files. Through training and testing this code, you'll witness just how powerful LSTM networks are and further understand the generative process. Good luck!


##Credits

The credits for this code go to [Ji Sung Kim](https://github.com/jisungk/deepjazz). I've merely created a wrapper to get people started.
