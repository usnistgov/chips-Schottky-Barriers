# chips-Schottky-Barriers
Data for a benchmark of Schottky barrier height (SBH) prediction at Si(111)/metal (Al, Cu, Ag, Au) interfaces. Compares XC functionals and bulk-reference protocols (relaxed, SOC, strained) and shows structural/electrostatic consistency drives SBH accuracy. Mixed hybrid–GGA + strained refs reach near-experimental SBHs at low cost.

This repository contains the atomic structures used in the study:
**Effect of Exchange-Correlation Functionals on Schottky Barriers at Si/Metal Interfaces**  
Viviana Dovale-Farelo and Kamal Choudhary
DOI: 10.1021/acs.jpcc.6c01668

The work investigates Schottky barrier heights (SBHs) at Si(111)/metal interfaces using first-principles density functional theory (DFT). The systems considered include Si(111) interfaced with Al, Cu, Ag, and Au surfaces. The structures provided here support the construction, relaxation, and analysis of the metal-semiconductor interfaces discussed in the manuscript.

# Repository Contents
This repository includes structural files for Si(111)/M interfaces, where: M = Al, Cu, Ag, Au.

The available interface orientations are:
- Si(111)/M(111)
- Si(111)/M(100)
- Si(111)/M(110)

The available interface configurations are:
- Original interface structures generated with INTERMAT.
- Relaxed interface structures using fixed-cell relaxation with ISIF=2.
The relaxed structures correspond to calculations in which the atomic positions were optimized while keeping the cell shape and volume fixed. This is consistent with the interface construction approach used in the study, where the semiconductor acts as the substrate and the metal film accommodates most of the lattice mismatch.

# Computational Details
The structures are intended for DFT calculations using VASP or compatible electronic-structure codes. In the study, the calculations were performed using:

- Code: VASP
- PAW method
- Plane-wave cutoff: 600 eV
- Interface k-point mesh: 7 × 7 × 1
- Interface relaxation: ISIF = 2

Several exchange-correlation functionals were evaluated in the manuscript, including:
- PBE
- OptB88vdW
- SCAN
- mBJ
- HSE06 (only for bulk references)







