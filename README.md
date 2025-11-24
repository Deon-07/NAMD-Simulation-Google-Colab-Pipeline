# NAMD 3 Simulation Pipeline (Colab + CUDA)

This repository contains a Google Colab notebook designed for running high-performance Molecular Dynamics (MD) simulations using **NAMD 3** with **CUDA acceleration**.

## Features

- **End-to-End Pipeline**: Handles Setup, System Configuration, Minimization, Equilibration, and Production.
- **Automated Configuration**: Dynamically generates NAMD `.conf` files based on user inputs.
- **Performance Optimized**:
  - Uses **CUDA** for GPU acceleration.
  - Optimizes CPU affinity and core usage.
  - Mitigates Google Drive I/O latency by writing logs locally.
- **Google Drive Integration**: Seamlessly mounts Drive for input files and automatic result backups.

## Usage

1.  **Upload to Drive**: Place your `.pdb`, `.psf`, and parameter files in a folder on Google Drive.
2.  **Open in Colab**: Upload `NAMD3_Simulation.ipynb` to Google Colab.
3.  **Configure**: Set your file paths and simulation parameters in the "System Configuration" cell.
4.  **Run**: Execute the cells to perform the simulation.

## Requirements

- Google Colab (Free or Pro) with GPU runtime (T4 recommended).
- NAMD 3 (downloaded automatically by the notebook).
- Valid PDB/PSF system files.
