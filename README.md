# DFT_workshop
QE tutorials for the workshop of Density Functional Theory course

## Requirements
1. Quantum ESPRESSO (QE) for electronic-structure calculations: https://www.quantum-espresso.org/
2. Basis Python libralies: Numpy, Matplotlib, Pandas, Sklearn
3. VESTA for visualization: https://jp-minerals.org/vesta/en/download.html

This workshop is in progress (Not yet completed).

## Projects
1. Phase Transition of Strontium (FCC to BCC) (optional)
  - Convergence testing of primitive fcc and bcc strontium.
  - SCF calculation
  - Pressure and Enthalpy calculation from E-V diagram
  - Outcome of this project: fcc-bcc phase transition diagram, Pressure at the transition point.
2. Electronic Band Gap of Diamond at High Pressure.
  - Available inputs : 
    - Structure example: primitive diamond, conventional diamond, and conventional diamond (a=3.0 Å).
    - Script example: Ecut convergence testing, kpoint convergence testing, and SCF calculations with variable a-parameter.
    - Input example: non-SCF calculation (a=3.0 Å), DOS calculation (a=3.0 Å), and Band calculation (a=3.0 Å).
    - Jupyter notebooks: convergence testing, reading the E-V diagram for pressure calculation, DOS plotting, and Band structure plotting.
  - Convergence testing of primitive diamond 
  - SCF calculation
  - Pressure calculation from the E-V diagram
  - non-SCF calculation
  - DOS calculation
  - Band structure calculation (optional)
  - Outcome of this project: DOS and band gap of Diamond at 0, 50, 100, and 150 GPa.
3. Electronic Properties of Boron Doped Diamond.
  - Available inputs : 
    - Structure example: conventional diamond and 3 structures of boron-doped conventional diamond.
    - Input example: vc-relax inputs of 4 structures.
  - Structure optimization (vc-relax) of conventional diamond (B0).
  - Structure optimization (vc-relax) of Boron doped diamond: 1atom doped (B1) and two configurations of 2atom doped (B2_1 and B2_2).
  - non-SCF calculation
  - DOS calculation
  - Outcome of this project: Relaxed structures, total energies, DOS, and band gap of 4 structures (B0, B1, B2_1, B2_2).
4. Magnetic Properties of BCC Iron(Fe).
  - Available inputs : 
    - Structure example: conventional iron.
    - Script example: relax calculations with variable a-parameter of nonmagnetic, ferromagnetic, and antiferromagnetic irons (non, fer, anti).
  - Convergence testing of conventional iron (nonmagnetic).
  - Structure optimization (relax) of nonmagnetic, ferromagnetic, and antiferromagnetic irons (non, fer, anti).
  - Outcome of this project: E-V diagram showing the magnetic properties of iron should be.

## Installing Quantum ESPRESSO

### on Ubuntu in Windows 
1. Download Ubuntu from Microsoft Store
2. Setup Subsystem (Linux) on Windows: please see http://aka.ms/wslinstall
3. Download QE on Ubuntu using the command "wget": wget https://github.com/QEF/q-e/releases/download/qe-7.0/qe-7.0-ReleasePack.tgz or wget https://gitlab.com/QEF/q-e/-/archive/qe-7.2/q-e-qe-7.2.tar.gz (latest version is 7.2 at the time of writing)
4. Un-tar the source files using the command "tar -zxvf": tar -zxvf q-e-qe-7.2.tar.gz
5. Change to the qe directory using the command "cd": cd q-e-qe-7.2
6. Issue (run) configure using the command "./": ./configure --> Waiting for "configure: success"
7. compile everything using the command "make all" or compile individual packages using the command "make ..." 
Now, the binary files or their symbolic links would be placed in the bin directory !!

** If you encounter a problem in the step "./configure": please try to install "gfortran": sudo apt-get install gfortran
** If you encounter a problem in the step "make all": please try to install "make-guile": sudo apt-get install make-guile

### on Terminal in MacOS
1. Open Terminal 
2. (Optional) Create environment: conda create —name “name of env”
3. Install homebrew: please see https://docs.brew.sh/Installation
4. Install these commands using the command "brew": brew install gcc open-mpi cmake wget
6. Download QE on Ubuntu using the command "wget": wget https://github.com/QEF/q-e/releases/download/qe-7.0/qe-7.0-ReleasePack.tgz or wget https://gitlab.com/QEF/q-e/-/archive/qe-7.2/q-e-qe-7.2.tar.gz (latest version is 7.2 at the time of writing)
7. Un-tar the source files using the command "tar -zxvf": tar -zxvf q-e-qe-7.2.tar.gz
8. Change to the qe directory using the command "cd": cd q-e-qe-7.2
9. Issue (run) configure using the command "./": ./configure --> Waiting for "configure: success"
10. compile everything using the command "make all" or compile individual packages using the command "make ..." 
Now, the binary files or their symbolic links would be placed in the bin directory !!

** If you encounter a problem in the step "make all": please see https://mattermodeling.stackexchange.com/questions/7146/installing-quantum-espresso-on-an-apple-m1-processor-possible

## Basic command lines on the terminal (bash)
- ls: Lists the files and directories in the current working directory
- cd: Changes the current working directory
- mkdir: Creates a new directory
- rm: Deletes a file or directory
- cp: Copies a file or directory
- mv: Moves or renames a file or directory
- cat: Displays the contents of a file
- grep: Searches for a pattern in a file or directory
- echo: Prints a message to the terminal
- pwd: Displays the current working directory
- sudo: Runs a command with root privileges
- chmod: Changes the permissions of a file or directory








