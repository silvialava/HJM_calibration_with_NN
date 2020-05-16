This repository contains the code used for the paper:

# Accuracy of Deep Learning in Calibrating HJM Forward Curves
(available soon)
by Fred Espen Benth, Nils Detering, Silvia Lavagnini.




We price European-style options written on forward contracts in the commodity market, which we model with a state-dependent infinite-dimensional Heath-Jarrow-Morton (HJM) approach. We introduce a new volatility operator which maps the square integrable noise into the Filipovic space of forward curves, and we specify a deterministic parametrized version of it. We train a neural network to approximate the option price as a function of the model parameters. We then use it to calibrate the HJM parameters starting from (simulated) options market data. Finally we introduce a new loss function taking into account bid and ask prices, providing a solution to the liquidity problem. A key issue discovered is that the trained neural network might be non-injective, which could potentially lead to poor accuracy in calibrating the forward curve parameters, even when showing high degree of accuracy in recovering the prices. This implies that the original meaning of the model parameters gets somehow lost in the approximation step.
