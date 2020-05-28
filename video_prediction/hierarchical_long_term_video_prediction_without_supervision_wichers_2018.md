Hierarchical Long-term Video Prediction without Supervision

# TLDR
Context: Popular video prediction approaches focus on recursively observing generated frames to 
make predictions further into the future (Mathieu et al., 2016; 
Goroshin et al., 2015; Srivastava et al., 2015; Ranzato et al., 2014; Finn et al., 2016; 
Villegas et al., 2017a; Lotter et al., 2017). However these approaches generate quality predictions
for the first few steps, but then the prediction dramatically degrades. Instead, a hierarchical
 method makes predictions in a high-level information hierarchy (e.g., landmarks) and then
decodes the predicted future in high-level back into low-level pixel space. The advantage
of predicting the future in high-level space first is that the predictions degrade less
quickly compared to predictions made solely in pixel space. 

Model approach: encode input frame, predict a high-level encoding into the future, and then a decoder
with access to the first frame produces the predicted image from the predicted encoding.

Training method: jointly train the encoder, the predictor and decoder together without 
high-level supervision. Additionally use an adversarial loss in the feature space to 
train the predictor.

Results: proposed method can predict 20 seconds into the future and provides better
results compared to Denton and Fergus - Stochastic video generation with a learned prior (2018)
 and Finn et. al - Unsupervised learning for physical interaction through physical interaction
 (2016).

# Key related papers
Denton and Fergus (2018) -  Stochastic video generation with a learned prior
Finn et. al (2016) - Unsupervised learning for physical interaction through video prediction
Babaeizadeh et. al (2018) - Stochastic variational video prediction
Srivastava et. al (2015) - Unsupervised learning of video representations using LSTMs
Villegas et. al (2017) -  Decomposing motion and content for natural video sequence prediction
Villegas et. al (2017) - Learning to generate long-term future via hierarchical prediction
Mathiey et. al (2016) - Deep multi-scale video prediction beyond mean square error
Goroshin et. al (2015) - Learning to linearize under uncertainty
Lotter et. al (2017) - Deep predictive coding networks for video prediction and unsupervised
learning
