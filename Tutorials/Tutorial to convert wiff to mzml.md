Experiments acquired on a SCIEX&reg; SelexION Differential Mobility Separation device (DMS) produces datafile in the format of .wiff and .wiff.scan files. 
Without using SCIEX&reg's proprietory softwares, experimental data can't be extracted from these files readily, which will hinder further analysis. DMS Data Extraction Toolkit
was created for the purpose of extracting DMS data in batch in an automatic manner.

This tutorial will guide users through steps to convert .wiff files to .mzml format. MZML format is an open-sourced, XML-formatted method of storing mass spectrometry data. Once converted to .mzml format, these files can then be extracted using the DMS Data Extraction Toolkit into a .csv format, ready for analyzed by
iDMS [link](https://github.com/Neurolipidomics/iDMS) or by other methods.

## Tutorial
**1.** Download Proteowizard
  - Access Proteowizard website at https://proteowizard.sourceforge.io/download.html.
  - Choose “Proteowizard” in “Project”.
  - Enter in the Download form the information appropriate to your computing platform.
  - Read and accept the license agreements to Download.
  - Install Proteowizard on your computer

**2.** Convert .wiff files to .mzml files
  - Open msconvert on your computer.
  - Select “List of Files”, then choose "Browse" (Figure below).

<img width="75%" height="75%" alt="wiff to mzml_Proteowizard 1" src="https://github.com/user-attachments/assets/f7a4a60d-ae25-4dd0-b558-2905352f191f" />

  - Navigate to each optimization folder, press and hold “Ctrl” (PC) or “Command” (Mac) to select all the .wiff files corresponding to that single optimization experiment (Figure below).

<img width="75%" height="75%" alt="wiff to mzml_Proteowizard 2" src="https://github.com/user-attachments/assets/6b4b2fc2-deec-4bfb-a396-717f8499abc7" />

  - Click “Open” when finished.
  - By default, the “Output Directory” is the same as the input directory (ie. the selected optimization folder). For file organization simplicity, leave this as default.
  - Choose “mzML” for Output format.
  - Binary encoding precision: 64-bit
  - Select: “Write index”, “Use zlib compression”, “TPP compatibility”.
  - Leave the rest as is.
  - Select “Start” in the bottom right corner.
  - Wait for the process to finish, as indicated in the “Conversion progress” window (Figure below).

<img width="75%" height="75%" alt="wiff to mzml_Proteowizard 3" src="https://github.com/user-attachments/assets/88bb4e2c-e4d5-42c0-b397-8db86a452782" />

  - Repeat the above steps with each optimization folder.
  - Each optimization folder now will have a .mzml file alongside the .wiff and .wiff.scan file for each optimization acquisition.

## References
(1) Orchard, S., Hermjakob, H., The HUPO proteomics standards initiative–easing com-munication and minimizing data loss in a changing world. Brief. Bioinformatics 2008,9, 166–173.\
(2) Deutsch, E., mzML: A single, unifying data format for mass spectrometer output. Proteomics 2008, 8: 2776-2777
