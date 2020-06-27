## Mobile Video Object Detection with Temporally-Aware Feature Maps - Liu and Zhu (2018)

####TLDR
Propose a series of modifications to LSTMs placed within single-frame oject detection models:
* Use of depth separable convolutions
* Bottleneck-LSTM which applies 1x1 convolution layer to the concatenated hidden state and input, 
to reduce the dimensions from (M + N) to N, i.e. same as the cell state.
* Use of ReLU in LSTM as activation function on cell state

**Key Results:**
* Stacking multiple LSTMs interspersed with convolutional layers only increases performance marginally
* Bottleneck LSTM gives comparable performance to normal LSTM or GRU
