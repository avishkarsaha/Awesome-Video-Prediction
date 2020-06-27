### PredRNN: Recurrent Neural Networks for Predictive Learning using Spatiotemporal LSTMs - Wang et al. (2017)

#### TLDR;
In typical ConvLSTMs, information passes vertically through every layer, and every layer is updated horizontally
(i.e. based on the layer's previous states). Here the authors add a "spatiotemporal" memory state to an LSTM cell
alongside its usual (what the authors call "temporal") cell state. In the proposed PredRNN, information within the unrolled graph of the LSTM flows
in two directions - the spatiotemporal memory flows in a sequential path vertically between layers (as if the layers
at every time step are stacked in a single column), while the cell state is passed between layers of each 
timestep as usual. The spatiotemporal memory state has the same equations as the cell state, and is concatenated 
with the temporal cell state and passed to the output gate.
