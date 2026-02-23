# Whispering Gallery Mode (WGM) Resonators - Simulation Study

## Project Overview: 

Computational study of Whispering Gallery Mode resonators — optical microresonators where light circulates near the surface via total internal reflection, analogous to the acoustic phenomenon first described by Lord Rayleigh (1878) at St. Paul's Cathedral.
What was simulated: A wedge-shaped SiO₂ microresonator modeled in COMSOL using an axisymmetric eigenfrequency solver. The geometry was surrounded by a Perfectly Matched Layer (PML) to absorb escaping radiation. The electric field was expressed as E(r,φ,z) = E(r,z)exp(−in_m φ), reducing the 3D problem to 2D.
<img width="822" height="457" alt="image" src="https://github.com/user-attachments/assets/34e123e4-6666-46f9-acf7-c701498986b7" />


In the idealized lossless case (κ=0), Q-factors reach ~10¹⁵
<img width="882" height="355" alt="image" src="https://github.com/user-attachments/assets/1630d576-1c5d-44b4-86b5-7a876b342382" />

Introducing material absorption (imaginary refractive index κ ~ 10⁻⁵ to 10⁻³) drops Q to 10⁴–10²
Adding a 50 nm silver coating reduces Q from 10¹⁵ to ~10⁴, with a sharp resonance peak near 278 THz, attributed to Ohmic heating, refractive index modification, and additional scattering:
<img width="1751" height="948" alt="image" src="https://github.com/user-attachments/assets/9bc77877-ef6f-4ce8-ad12-52da048e1f59" />


Tools: COMSOL Multiphysics (FEM eigenfrequency analysis)

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

The image below shows the Electric field distribution in 2D view: 

<img width="768" height="603" alt="electric_field_height_exp_2d_view" src="https://github.com/user-attachments/assets/a085f234-a452-4c0e-9ad0-917ab9951aef" />

It demonstrates the mode confinement within the high-index core. 
The best coupling condition in th erange 3.0um to 4.2um corresponds to 4.2um. 
The Electric field distribution along y-direction is computed to be the following: 
<img width="768" height="603" alt="Electric field norm along y" src="https://github.com/user-attachments/assets/f63ae0b9-068d-4fc9-9165-b155a3f17d7f" />
This shows that even though the material imaginary refractive index is set to 0, it still suffers high losses. 
