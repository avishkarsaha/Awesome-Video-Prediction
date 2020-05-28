High Fidelity Video Prediction with Large Stochastic Recurrent Neural Networks - Villegas et.
al (2019)

# TLDR
Previous approaches to video prediction require complex inductive biases inside network 
architectures with highly specialized computation, including segmentation masks, 
optical flow, and foreground and background separation. 

This proposal questions whether such handcrafted architectures are necessary and instead 
propose a different approach: finding minimal inductive bias for video prediction while 
maximizing network capacity.

Key results:
1. large models with mimimal inductive bias tend to improve performance both qualitatively 
and quantitatively.
1. recurrent models outperform non-recurrent models
1. stochastic models perform better than non-stochastic models, especially in the 
presence of uncertainty. 
