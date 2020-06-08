Probabilistic Video Prediction from Noisy Data with a Posterior Confidence - Wang et. al (2020)

# TLDR
Study a new research problem of probabilistic future frames prediction from a sequence of 
noisy inputs using an end-to-end trainable model named Bayesian Predictive Network (BP-Net).
Unlike previous work in stochastic video prediction that assumes spatiotemporal coherence
and therefore fails to deal with perceptual uncertainty, BP-Net models both levels of 
uncertainty in an integrated framework. Furthermore, unlike previous work that can only 
provide unsorted estimations of future frames, BP-Net leverages a differentiable sequential
importance sampling spproach to make future predictins based on the inference of 
underlying physical states.
