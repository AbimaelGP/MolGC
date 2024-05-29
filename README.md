# MolGC
MolGC: Molecular Geometry Comparator Algorithm for Bond Length Mean Absolute Error Computation on Molecules

![image](https://github.com/AbimaelGP/MolGC/assets/167240268/99c9a283-d1c8-4ee2-8685-5f0e09364993)

## This paper is currently under review

# Desrciption of the repository

This repository hosts a collection of molecular geometry files generated using Density Functional Theory (DFT) or ab-initio methods. These files will be used for comparative analysis of mean absolute bond lengths. Additionally, the repository includes the executable file (.exe) for the MolGC software.

# Instructions:

## 1)Prepare your files

Ensure to add a folder named "Molecules" inside the main folder.

Example: C:\Users\Assigned User\Desktop\Mainfolder\Molecules

The Molecules folder has five levels of folders:

First level: The first folders are named according to a family of molecules to be evaluated. In this example, we include several molecular families used in our study, specifically antibiotics. These families are Nitrofurans, Quinolones, and Fluoroquinolones.

Second level: Inside the folders of each antibiotic family are specific folders for each different type of antibiotic. For example, within the Fluoroquinolones folder, there are folders corresponding to antibiotics like ciprofloxacin, enoxacin, fleroxacin, etc.

Third level: Inside each specific antibiotic folder are folders named according to the software used to obtain its minimum energy geometry. For example, within the ciprofloxacin folder, there are folders: CASTEP, FHI-aims, and Gaussian, which correspond to three different software used to obtain the geometry of the ciprofloxacin molecule.

Fourth level: Inside the CASTEP, FHI-aims, or Gaussian folders are folders corresponding to different levels of theory to obtain the minimum energy geometry. For example, for the CASTEP software, the theory levels evaluated are LDA, LDA+OBS, PBE, and PBE+TS. Therefore, there is a folder for each of these functionals.

Fifth level: Finally, inside the folders of each different theory level (e.g., LDA, LDA+OBS, PBE, and PBE+TS) is a file with the extension .castep, .out, or .log (extension .xyz is also supported, see example of Molecules-Crystals files in this repository).These files contain information about the spatial coordinates of the optimized geometry of the molecules. These files are processed to compare geometries at different theory levels, thereby performing statistical analysis on their variations and the absolute error percentage concerning the reference molecule. This referece can be selected from software menu.

## 2)Download MolGC software

Ensure to add a folder named "SoftwareMolGC" inside the main folder.

Example: C:\Users\Assigned User\Desktop\Mainfolder\SoftwareMolGC

Download the .exe file from:
[https://drive.google.com/file/d/1LIWz2i9R6OR2iskV27tD4KlR1kloa0h3/view?usp=sharing](https://drive.google.com/file/d/1LIWz2i9R6OR2iskV27tD4KlR1kloa0h3/view?usp=sharing)

Place the executable Main.exe file inside the "SoftwareMolGC" folder.

## 3)Initiate Your Comparative Analysis.

Attention: We recommend disabling your computer's antivirus software so that it does not recognise the Main.exe program as a threat.

Run the Main.exe to start making comparisons and give the reference when requested by the programme. 

If everything goes well, a folder called Files should be created in the main menu:
Example: C:\Users\Assigned User\Desktop\Mainfolder\Files

The "Files" folder will contain visual and graphical information about the error generated during comparisons for each molecule and family.
For example, after running the program at the path: 
C:\Users\Assigned User\Desktop\Mainfolder\Files\FLUOROQUINOLONES\ciprofloxacin_files

The following files are found: ciprofloxacin.html, ciprofloxacin_Structure.html, Table_MAE_ciprofloxacin.xlsx

- 	The ciprofloxacin.html file contains 3D graphs of absolute error percentage statistics.
- 	The ciprofloxacin_Structure.html file contains an interactive 3D visualization of the molecules compared. It allows for verifying the correct overlap and the bonds and different elements evaluated.
- 	The Table_MAE_ciprofloxacin.xlsx file contains numerical information on the comparisons made for each bond of the different functionals.

Graphical and document information in Excel format is also available by molecule family.
For example, at the path: C:\Users\Assigned User\Desktop\Mainfolder\Files\FLUOROQUINOLONES

The following files are found: MAE_perfamily_permolecule.html and Table_MAE_general.xlsx

- The MAE_perfamily_permolecule.html file contains 3D graphs of average absolute error percentage statistics by molecule family.
- The Table_MAE_general.xlsx file contains numerical information on the average error of the comparisons made for each bond of the different functionals by molecule family.

Finally, within the 'Files' folder or path: C:\Users\Assigned User\Desktop\Mainfolder\Files, the file MAE_general.html is found.

- The MAE_general.html file contains 3D graphs of average absolute error percentage statistics for all evaluated molecule families.

![image](https://github.com/AbimaelGP/MolGC/assets/167240268/1084a936-8de2-4e61-aac3-6b70e0a2aed2)

