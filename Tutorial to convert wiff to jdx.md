Experiments acquired on a SCIEX&reg; SelexION Differential Mobility Separation device (DMS) produces datafile in the format of .wiff and .wiff.scan files. 
Without using SCIEX&reg's proprietory softwares, experimental data can't be extracted from these files readily, which will hinder further analysis. DMS Data Extraction Toolkit
was created for the purpose of extracting DMS data in batch in an automatic manner.

This tutorial will guide users through steps to convert .wiff files to .jdx (JCAMP-JDX) format. JCAMP-JDX format is a manufacturer-independent method of storing and 
sharing spectroscopic data. Once converted to .jdx format, these files can then be extracted using the DMS Data Extraction Toolkit into a .csv format, ready for analyzed by
iDMS [link](https://github.com/Neurolipidomics/iDMS) or by other methods.

## Tutorial
**Requirement**: User must have already installed Analyst software version 1.6.2 or 1.6.3 from SCIEX&reg website.\

Both Sciex® Analyst software versions 1.6.2 and 1.6.3 come with supplemental scripts which can be found in the Scripts folder, often found in one’s computer 
at C:\Program Files (or Program Files (x64) of (x86))\Analyst\Scripts. In this folder, look for the script folder “BatchScriptDriver”.

1. Enter the folder BatchScriptDriver\Install.
2. Double-click “BatchScriptDriver.exe”
3. In box “Script”, select “Select…”, navigate to the Scripts folder, and select the script folder “Export To JCamp”, enter folder and subfolder “Install.
4. Choose file “Export To JCamp.dll”. Click “Open” to select (Figure below).


<img width="4400" height="1245" alt="wiff to jdx 1" src="https://github.com/user-attachments/assets/71140d86-8102-4b5e-9789-79cab363d9bf" />


5. In box “Files to Process”, add the folder containing your acquisition files by choosing “Add folder…” and navigate to the right directory. \
Note that, if you performed experiment with multiple lipid isomers, you can select the parent folder which stores individual folder of each optimization experiment. 
This script will allow the conversion to be carried out in batch (Figures below).

<img width="2329" height="1245" alt="wiff to jdx 2a" src="https://github.com/user-attachments/assets/2bbd074b-eae9-44e8-b29f-9bf6e3038358" />

<img width="1188" height="1245" alt="wiff to jdx 2b" src="https://github.com/user-attachments/assets/3150f4bb-0238-4fae-8746-05f2b171364c" />

6. Click “Run” to start the process.
7. A small window will pop up prompting for “Options”. The following settings are recommended, however, change these settings should you wish to match your experiment:
  - Intensity Threshold: 3
  - Select “Centroid Exported Spectra”
  - In box for “Field”, choose “Intensity”
  - Select “Deisotope”
  - Unselect “Only show this dialog again if the control key is down”.

<img width="2159" height="1245" alt="wiff to jdx 2c" src="https://github.com/user-attachments/assets/d294625b-e00b-45db-a038-0eb4fd260565" />

>[!Note]
>Although nothing seems to indicate that the script is working, it is indeed working in the background. New .jdx files will show up in the folder of each optimization experiment for each acquisition. You can monitor the progress of this script running by checking when all data folders now contain a .jdx file for each .wiff file. Then, close the application.



