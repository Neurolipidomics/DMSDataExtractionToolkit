DMS Data Extraction Toolkit was created to enable users to easily batch extract data from .jdx or .mzml files and populate .csv sample datasets in the format used by [iDMS](https://github.com/Neurolipidomics/iDMS).

DMS data collected on a Sciex® SelexION Differential Mobility Separation device is acquired in proprietary .wiff and .wiffscan format.  These data can be converted to .jdx or .mzml files for batch processing using the DMS Data Extraction Toolkit. JCAMP-DX is an ASCII-based format (1-3). MZML is an open-source XML-based format (4,5).  Both formats are used to store and share mass spectrometry data across platforms and manufacturers.

This tutorial is meant as a helpful guide for users new to transforming Sciex®  .wiff and .wiffscan to .jdx using their existing Analyst software.


## Tutorial
**Requirement**: User must have already installed Analyst software version 1.6.2 or 1.6.3 from Sciex® website.

Both Sciex® Analyst software versions 1.6.2 and 1.6.3 come with supplemental scripts which can be found in the Scripts folder, often found by default at C:\Program Files (or Program Files (x64) or (x86))\Analyst\Scripts). Once you have located this folder, look for the script folder “BatchScriptDriver”.

1. Enter folder BatchScriptDriver\Install.
2. Double-click “BatchScriptDriver.exe”.
3. In box “Script”, select “Select…”, navigate to the Scripts folder, and select the script folder “Export To JCamp”, enter folder and subfolder “Install".
4. Choose file “Export To JCamp.dll”. Click “Open” to select (Figure below).

<img width="4400" height="1245" alt="wifftojdx_step1" src="https://github.com/user-attachments/assets/5a0f2360-b7d8-4b86-afa0-20192a65ad94" />

5. In box “Files to Process”, add the folder containing your acquisition files by choosing “Add folder…” and navigate to the right directory.
   
Note that, if you performed experiment with multiple lipid isomers, you can select the parent folder which stores individual folder of each optimization experiment. This script will allow the conversion to be carried out in batch (Figure below).

<img width="80%" height="80%" alt="wiff to jdx 2a" src="https://github.com/user-attachments/assets/2bbd074b-eae9-44e8-b29f-9bf6e3038358" />

<img width="40%" height="40%" alt="wiff to jdx 2b" src="https://github.com/user-attachments/assets/3150f4bb-0238-4fae-8746-05f2b171364c" />

6. Click “Run” to start the process.
7. A small window will pop up called “JCamp Options”. The following settings have been tested, however, all settings can be changed according to user input:
    - Intensity Threshold: 3
    - Select “Centroid Exported Spectra”.
    - In box for “Field”, choose “Intensity”.
    - Select “Deisotope”.
    - Unselect “Only show this dialog again if the control key is down”.

<img width="75%" height="75%" alt="wiff to jdx 2c" src="https://github.com/user-attachments/assets/d294625b-e00b-45db-a038-0eb4fd260565" />

> [!Note]
> Although nothing will indicate that the script is working, files are being exported in the background. New .jdx files will show up in the folder containing each optimization experiment for each acquisition. The process is complete when all data folders contain a .jdx file for each .wiff file. Once completed, close the application.

## References
(1) Gasteiger, J., B. M. P. Hendricks, Hoever P., Jochum C., and Somberg H. 1991. “JCAMP-CS: A Standard Exchange Format for Chemical Structure Information in a Computer-Readible Form.” Applied Spectroscopy 45 (1): 4–11.\
(2) Lampen, P, H Hillig, AN Davies, and M Linscheid. 1994. “JCAMP-DX for Mass Spectrometry.” Applied Spectroscopy 48 (12): 1545–52.\
(3) Baumbach, JI, AN Davies, P Lampen, and H Schmidt. 2001. “JCAMP-DX. A Standard Format for the Exchange of Ion Mobility Spectrometry Data - (IUPAC recommendations 2001).” Pure and Applied Chemistry 73 (11): 1765–82.\
(4) Orchard, S., Hermjakob, H., The HUPO proteomics standards initiative–easing com-munication and minimizing data loss in a changing world. Brief. Bioinformatics 2008,9, 166–173.\
(5) Deutsch, E., mzML: A single, unifying data format for mass spectrometer output. Proteomics 2008, 8: 2776-2777.






