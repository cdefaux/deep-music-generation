# Capstone
Deep Learning Techniques for Music Generation

This is my final project for the Flatiron Data Science immersive. I decided to tackle music generation and dig deep in my exploration of the possibilities. There is a panoply of model types and techniques that can be used to analyse and generate music. One certainty is that music generation is the goal rather than a classification problem. Therefore, for the purposes of building a model, generative rather than discriminative models will be investigated. Perhaps a problem for a later date would be to build a discriminative music genre classifier, however, I imagine this could be quite difficult and would require training the model on a massive corpus of music of all genres.

## Introduction

During my exploration of the field I found many papers outlining different techniques for music generation. One particularly useful document was "Deep Leaning Techniques for Music Generation" (Briot et al., 2019), which outlines the various data structures for music encoding, then delves into various neural network architectures and examples of specific models. 

There have been myriad attempts at generating music, with varied success (in my opinion). Something pertinent to music is the subjectivity of the material. What does one consider 'good' music? This subjectivity adds complexity when evaluating a seemingly arbitrary sample. Music is very deliberate, therefore, I imagine a computer will struggle to create human-sounding pieces. Music tells a story and conveys emotion meaning that a computer inherently cannot understand those dimensions. The symbiosis of human and computer could allow for realistic and emotive expressions. It will be interesting to see where computer generated music will go when pre-mapped by humans.

Those who may not yet understand deep learning; it is a machine learning technique based on artificial neural networks. A deep (excuse the pun) explanation is out of the scope of this document, however as a high level abstraction, one can imagine a neural network or "brain" that is fed large volumes of data and learns the intrinsic patterns of that data. Artificial Neural Networks (ANNs) were inspired by information processing and distributed communication nodes in biological systems. What makes those ANNs deep (DNN) is the additional layers between the input and output layers. Some tasks which deep learning can be used for are: facial recognition, text recognition, sentiment analysis and many others. Within deep learning there are myriad neural network architectures which can be used for various problems.

For the purposes of generation, the DNN architecture will depend on the audio format. For image data, the Convolutional Neural Network (CNN/ConvNet) architecture will be most useful as it is able to recognize features in images very well. Another option would be to use a Recurrent Neural Network (RNN) which is basically a model that self-recurs and thereby is able to model sequential data very effectively. Autoencoders present another possible architecture. An autoencoder works by compressing input data into a smaller bottleneck hidden layer with fewer nodes than the input. Finally, one simple but possibly useful model is the Restricted Boltzmann Machine (RBM) which is a variation on a neural network that has only 2 layers, an input/output and a hidden layer. 

Further, the question of data format for the project is a salient one. The project goals and scope will determine formatting. As mentioned above, the options are varied and require very different architectures. Firstly, one must consider the difference between symbolic and audio. Symbolic being the note and beat representations and audio being a direct representation of the raw audio wave. Within the symbolic sphere, some options are MIDI (Music Instrument Digital Interface - data produced by MIDI/electronic instruments, piano roll (an unrolled representation of melody based on punch-holed roll for automatic pianos), text (musical notes from A to G) among many others. In the other sphere of audio, two main types of raw audio representation can be used: raw audio waveform (.wav file) and spectrogram (a transformation of the audio wave into frequency, amplitude and time. 

Each of these data types present their own challenges and benefits. A large challenge is the 
