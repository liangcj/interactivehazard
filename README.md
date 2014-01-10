Interactive non-parametric hazard estimation
============================================
A D3.js demo using the well-worn PBC Mayo data (n=312). Non-parametric conditional hazard estimation with interactive marker-bandwidth selection! Time-bandwidths are hard-coded for now.

Potential uses:

* Univariate data exploration
* Evaluating the proportional hazards assumption
* Bandwidth selection

Computations are all done in the browser. Estimation is done by calculating Nelson-Aalen cumulative hazard, then smoothing it using the Epanechnikov kernel.

Scaling up to ~700 observations did not affect performance. Scaling up to ~18000 noticeably affected performance but was still usable. This was on a laptop with an Intel i7-3517U processor ([2012 consumer-grade mobile processor](http://ark.intel.com/products/65714/)). As would be expected, RAM usage and disk speed did not appear to be limitations.

To-do list:

* Labels for graphs
* Add more annotations/descriptions
* Option to vary time-bandwidth
* Change marker-bandwidth to Epanechnikov too (with accompanying alpha shading!)