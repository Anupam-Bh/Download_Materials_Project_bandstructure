# Download_Materials_Project_bandstrcutre

This script downloads bandstructures from Materials Project within a given range of material-id. The starting id is to be given in the 'data_index' file as a sinle digit. This file updates after every iteration. The final id is given in the script.sh file. 

Prerequisites:
1. Pymatgen must be installed as an anaconda package. Change 11-12th line to match your system. 
2. You must get a MPRester-ID. This has to be obtained from the Materials Project website. Update this ID inside the quotes in line 33.

Each image will be saved in PNG format with a fixed resolution of 250X150. 
For facilitating image based ML applications, the bandstructures are stripped of every feature except the curves of the bands. However, a horizontal line at the Fermi energy will still be present and to remove that one need to edit '~/anaconda3/envs/pymatgen/lib/python3.9/site-packages/pymatgen/electronic_structure/plotter.py'
The final image will look like following:
![mp-223_GeO2](https://user-images.githubusercontent.com/106304435/170889176-e9279f92-f057-4cb6-9531-90a100e7fd45.png)
