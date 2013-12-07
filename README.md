Interactive non-parametric hazard estimation
============================================
A D3.js demo using the well-worn PBC Mayo data. Non-parametric conditional hazard estimation with interactive marker bandwidth selection! Time-bandwidths are hard-coded for now.

Computations are all done in the browser. Estimation is done by calculating Nelson-Aalen cumulative hazard, then smoothing it using the Epanechnikov kernel.