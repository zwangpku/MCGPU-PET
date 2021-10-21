## NOTE: The MCGPU-PET code is not yet cleared for online distribution. The original MCGPU code for x-ray imaging is available at https://github.com/DIDSR/MCGPU. Come back soon or "watch" this repository for updates on the code availability. You can also use the Issues tab for contacting the developers. Thanks!

# MCGPU-PET: Open-Source Real-Time Monte Carlo PET Simulator

Monte Carlo (MC) simulations are used to model the emission, transmission, and detection of the radiation in Positron Emission Tomography (PET). In this work we introduce a new open-source MC software for PET simulation, MCGPU-PET, which has been designed to fully exploit the computing capabilities of modern GPUs to be able to simulate the acquisition of up to 1 million coincidences per second from voxelized source and material distributions. We evaluated the performance of the code, and applied it to provide fast accurate estimation of the PET coincidences (trues, scatter, randoms, and spurious coincidences). We simulated the numerical Zubal head phantom, using 8 different tissues, assuming a standard 18F-FDG uptake. A fully-3D scatter sinogram with 10 million coincidences was generated in 13 seconds in one GPU, indicating that the code might be fast enough to be used within an iterative image reconstruction process. MCGPU-PET provides estimation of True and Scatter coincidences and spurious background for non-standard isotopes at a rate 3 orders of magnitude faster than standard MC methods. This significant speed-up makes it a good candidate for providing accurate Scatter estimations within the image reconstruction process.

Authors:


- **Andreu Badal** [DIDSR, OSEL, CDRH, US Food and Drug Administration, Silver Spring, MD]
- **Joaquin L. Herraiz** and  **Alejandro López-Montes** [Complutense University of Madrid, EMFTEL, Grupo de Fisica Nuclear and IPARCOS, Madrid, Spain; Instituto de Investigacion Sanitaria del Hospital Clinico San Carlos (IdiSSC), Madrid, Spain]

---

Code presented at the IEEE NSS MIC conference (https://nssmic.ieee.org/2021/) on October 21, 2021:

- **M-07-01 – GPU-accelerated Monte Carlo-Based Scatter and Prompt-Gamma Corrections in PET**, A. López-Montes, J. Cabello, M. Conti, A. Badal, J. L. Herraiz


---

# Disclaimer
This software and documentation (the "Software") were developed at the Food and Drug Administration (FDA) by employees of the Federal Government in the course of their official duties. Pursuant to Title 17, Section 105 of the United States Code, this work is not subject to copyright protection and is in the public domain. Permission is hereby granted, free of charge, to any person obtaining a copy of the Software, to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, or sell copies of the Software or derivatives, and to permit persons to whom the Software is furnished to do so. FDA assumes no responsibility whatsoever for use by other parties of the Software, its source code, documentation or compiled executables, and makes no guarantees, expressed or implied, about its quality, reliability, or any other characteristic. Further, use of this code in no way implies endorsement by the FDA or confers any advantage in regulatory decisions. Although this software can be redistributed and/or modified freely, we ask that any derivative works bear some notice that they are derived from it, and any modified versions bear some notice that they have been modified.
