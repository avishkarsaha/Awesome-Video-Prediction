Memory in Memory: A predictive neural network for learning higher-order non-stationarity 
from spatiotemporal dynamics - Wang et al (2019)

# TLDR
Propose Memory-in-Memory (MIM) blocks which exploit the differential signals between adjacent recurrent
states to model the non-stationary and approximately stationary properties in spatiotemporal 
dynamics.

Using Cramer's Decomposition, any non-stationary process can be decomposed into deterministic, 
time-variant polynomials and a zero-mean stochastic term. By applying differencing operations, 
the time-variant polynomials can be turned into a constant, making the deterministic component
predictable. However, most RNNs for spatiotemporal prediction do not use the differential signals
effectively, and their simple state transition functions prevent them from learning complex
variations in spacetime. 


