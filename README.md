This repository contains the code used for the paper:

# Accuracy of Deep Learning in Calibrating HJM Forward Curves
available at: https://arxiv.org/abs/2006.01911
by Fred Espen Benth, Nils Detering, Silvia Lavagnini.


We price European-style options written on forward contracts in a commodity market, which we model with a state-dependent infinite-dimensional Heath-Jarrow-Morton (HJM) approach. We introduce a new class of volatility operators which map the square integrable noise into the Filipovic space of forward curves, and we specify a deterministic parametrized version of it. For calibration purposes, we train a neural network to approximate the option price as a function of the model parameters. We then use it to calibrate the HJM parameters starting from (simulated) option market data. Finally we introduce a new loss function that takes into account bid and ask prices and offers a solution to calibration in illiquid markets. A key issue discovered is that the trained neural network might be non-injective, which could potentially lead to poor accuracy in calibrating the forward curve parameters, even when showing a high degree of accuracy in recovering the prices. This reveals that the original meaning of the parameters gets somehow lost in the approximation.
