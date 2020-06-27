Bayesian Prediciton of Future Street Scenes using Synthetic Likelihoods

TLDR
When anticipating future scenes, future states become increasingly uncertain and multi-modal, particularly on long 
time horizons. Although dropout based Bayesian inference provides a computational tractable approach to learn models, 
such approaches often fall short if deterministic approaches as the log-likelihood estimate used discourages
diversity. 

This work proposes a novel Bayesian formulation for anticipating future scenes which leverages synthetic
likelihoods that encourage the learning of diverse models to accurately capture the multi-modal nature
of future scenes. The approach achieves state-of the art predictions and calibrated probabilities 
on Cityscapes.


