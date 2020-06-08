Recurrent Flow-Guided Semantic Forecasting - Terwilliger et. al (2018)

# TLDR
Decompose the semantic forecasting task into two subtasks: current frame-segmentation and future
optical flow prediction. The proposed approach aggregates past optical flow features using 
a convolutinal LSTM to predict future optical flow, which is used by a learnable warp layer
to produce future segmentation.

Training method: supervision signal comes only from semantic segmentation masks
