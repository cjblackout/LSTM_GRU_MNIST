# LSTM_MNIST
Implementation of LSTM Cells for MNIST Classification


This repository contains two implementations of MNIST classification using Recurrent Neural Network methodologies which can be classified as follows

1. Long Short Term Memory (http://www.sciencedirect.com/science/article/pii/S0893608005001206)
It features three gates (input, forget, output), block
input, a single cell (the Constant Error Carousel), an output
activation function, and peephole connections1. The output of
the block is recurrently connected back to the block input and
all of the gates.

![alt text](https://github.com/cjblackout/LSTM_MNIST/blob/master/LSTM.JPG)

2. Gated Recurrent Unit (http://www.wildml.com/2015/10/recurrent-neural-network-tutorial-part-4-implementing-a-grulstm-rnn-with-python-and-theano/)
A GRU has two gates, a reset gate r, and an update gate z.  
Intuitively, the reset gate determines how to combine the new input with the previous memory, 
and the update gate defines how much of the previous memory to keep around. 
If we set the reset to all 1’s and  update gate to all 0’s we again arrive at our plain RNN model. 

![alt text](https://github.com/cjblackout/LSTM_MNIST/blob/master/Comparison.JPG)

The training accuracy for both networks reached 1.00 after 10,000 training steps. The testing accuracy of the LSTM cell was 0.992 while that of the GRU cell was 1.00 on learning rate 0.001, batch size 128 and the number of hidden layers being 128 as well.
