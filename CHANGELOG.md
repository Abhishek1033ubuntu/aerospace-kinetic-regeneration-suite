# Changelog

All notable changes to the **Aerospace Kinetic Regeneration Suite** will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

---

## [1.0.0] - 2026-10-10

### Added
* **Multi-Physics Differential Simulation Engine (`simulations/kinetic_recovery_sim.py`):**
  * Solved $12\text{ ms}$ transient torque absorption dynamics utilizing a parallel $15.8\text{ F} / 900\text{ V}$ ultracapacitor bank.
  * Formulated Euler differential thermal integration ($\Delta T = \frac{P \cdot dt}{C_{\text{thermal}}}$) incorporating dynamic ram-air convection ($h \propto v^{0.8}$) and Cu-Diamond MMC heat sinks.
  * Implemented $15\text{ kHz}$ SiC MOSFET active back-EMF ABS-analogy pulsing logic, holding peak stator temperatures to $64.3^\circ\text{C}$ under $1.2\text{G}$ emergency braking.
* **Interactive Google Colab Notebook (`simulations/kinetic_recovery_sim.ipynb`):**
  * Created a 2-cell error-guarded notebook architecture containing interactive visualization charts and environment setup.
* **Documentation & Case Studies:**
  * Added `docs/CASE_02_KINETIC_RECOVERY_LOSSES.md` detailing full Bill of Materials (BOM) cost delta and engineering benchmarks.
  * Cross-referenced `docs/CASE_01_MODERATE_FREQ_FSI.md`.
* **Publishing Infrastructure:**
  * Configured `.github/workflows/python-simulation-ci.yml` for automated CI build verification.
  * Added `.github/FUNDING.yml`, `CITATION.cff`, and open-source badges.
