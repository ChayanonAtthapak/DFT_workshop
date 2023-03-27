# DFT_workshop
QE tutorials for workshop of Density Functional Theory teaching

**Requirements**
1. Quantum ESPRESSO (QE) for electronic-structure calculations: https://www.quantum-espresso.org/
2. Basis Python libralies: Numpy, Matplotlib, Pandas, Sklearn
3. VESTA for visualization: https://jp-minerals.org/vesta/en/download.html

This workshop is in progress (Not yet completed).

**Projects**
1. Phase Transition of Strontium (FCC to BCC)
  (...)
2. Electronic Band Gap of Diamond at High Pressure
  - Available inputs : 
    - Structure example : premitive diamond, conventional diamond, and conventional diamond (a=3.0 Å)
    - Script example : Ecut convergence testing, kpoint convergence testing, and adjusting a parameter SCF calculation
    - Input example : non-SCF calculation (a=3.0 Å), DOS calculation (a=3.0 Å), and Band calculation (a=3.0 Å)
    - Jupyter notebooks : convergence testing, Reading E-V diagram for pressure calculation, DOS plotting, and Band structure plotting
  - Convergence testing of premitive diamond 
  - SCF calculation
  - Pressure calculation from E-V diagram
  - non-SCF calculation
  - DOS calculation
  - Band structure calculation (optional)
  - Outcome of this project: DOS and band gap of Diamond at 0, 50, 100 and 150 GPa
3. Electronic Properties of Boron Doped Diamond
  - Available inputs : 
    - Structure example : conventional diamond and 3 structures of boron doped conventional diamond 
    - Input example : vc-relax inputs of 4 structures
  - Structure optimization (vc-relax) of conventional diamond (B0)
  - Structure optimization (vc-relax) of Boron doped diamond : 1atom doped (B1) and two configuration of 2atom doped (B2_1 and B2_2)
  - non-SCF calculation
  - DOS calculation
  - Outcome of this project: Relaxed structures, total energies, DOS and band gap of 4 structures (B0, B1, B2_1, B2_2)
4. Magnetic Properties of BCC Iron(Fe)
  (...)
