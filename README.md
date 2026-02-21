# Microring-Resonator-in-MIR

## Project Overview

This repository details the design and simulation of a microring resonator optimized for operation in the mid-infrared (MIR) spectral region. Microring resonators are fundamental components in integrated photonics, crucial for applications such as sensing, spectroscopy, and optical filtering. This project specifically explores the adaptation of a microring design to MIR wavelengths, potentially leveraging **Magnesium Fluoride (MgF2)** for its transparency and refractive index properties in the MIR.

## Design Parameters for MIR Operation

The microring resonator was designed by adapting parameters from a near-infrared (NIR) design to the MIR, specifically targeting a central wavelength of **4.1 µm**.

*   **Operating Wavelength (`wl0_new`):** [e.g., 4.0 µm]
*   **Core Material:** [e.g., Silicon (Si) or MgF2] with a refractive index of `n_core_new = [Insert value, e.g., 3.43 for Si at 4µm or 1.375 for MgF2]`
*   **Cladding Material:** [e.g., Magnesium Fluoride (MgF2) or Air] with a refractive index of `n_clad_new = [Insert value, e.g., 1.375 for MgF2 or 1.0 for Air]`
*   **Core Width (`w_core_new`):** [e.g., 0.516 µm]
*   **Cladding Width (`w_clad_new`):** [e.g., 5.16 µm]
*   **Radius of Curvature (`r0_new`):** [e.g., 16 µm]
*   **Waveguide Separation (`dx_new`):** [e.g., 1.849 µm]

The image below shows the Electric field distribution in 3D view: 

<img width="1063" height="603" alt="electric_field_height_exp" src="https://github.com/user-attachments/assets/f1e49425-655c-487e-b385-5ad3bb9fc32e" />

It demonstrates the mode confinement within the high-index core. 
