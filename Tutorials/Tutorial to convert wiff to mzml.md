DMS Data Extraction Toolkit was created to enable users to easily batch extract data from .jdx or .mzml files and populate .csv sample datasets in the format used by [iDMS](https://github.com/Neurolipidomics/iDMS).

DMS data collected on a Sciex® SelexION Differential Mobility Separation device is acquired in proprietary .wiff and .wiffscan format.  These data can be converted to .jdx or .mzml files for batch processing using the DMS Data Extraction Toolkit. JCAMP-DX is an ASCII-based format (1-3). MZML is an open-source XML-based format (4,5).  Both formats are used to store and share mass spectrometry data across platforms and manufacturers.

This tutorial is meant as a helpful guide for users new to transforming Sciex®  .wiff and .wiffscan to .mzml using their existing Analyst software.


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

  - Navigate to each optimization folder, press and hold “Ctrl” (PC) to select all the .wiff files corresponding to that single optimization experiment (Figure below).

<img width="75%" height="75%" alt="wifftomzml_step2" src="https://github.com/user-attachments/assets/5319a2bf-3928-46a5-b2b3-cd2ad3b1d857" />

  - Click “Open” when finished.
  - By default, the “Output Directory” is the same as the input directory (ie. the selected optimization folder). For file organization simplicity, leave this as default.
  - Choose “mzML” for Output format.
  - Binary encoding precision: 64-bit
  - Select: “Write index”, “Use zlib compression”, “TPP compatibility”.
  - Leave the rest as is (default).
  - Select “Start” in the bottom right corner.
  - Progress is indicated in the “Conversion progress” window (Figure below).

<img width="75%" height="75%" alt="wifftomzml_step3" src="https://github.com/user-attachments/assets/bbd9965a-d710-4973-aa53-dc52b8d133d6" />

  - Repeat the above steps for each optimization folder.
  - Each optimization folder now will have a .mzml file as well as the original .wiff and .wiff.scan files for each optimization acquisition.

## References
(1) Gasteiger, J., B. M. P. Hendricks, Hoever P., Jochum C., and Somberg H. 1991. “JCAMP-CS: A Standard Exchange Format for Chemical Structure Information in a Computer-Readible Form.” Applied Spectroscopy 45 (1): 4–11.\
(2) Lampen, P, H Hillig, AN Davies, and M Linscheid. 1994. “JCAMP-DX for Mass Spectrometry.” Applied Spectroscopy 48 (12): 1545–52.\
(3) Baumbach, JI, AN Davies, P Lampen, and H Schmidt. 2001. “JCAMP-DX. A Standard Format for the Exchange of Ion Mobility Spectrometry Data - (IUPAC recommendations 2001).” Pure and Applied Chemistry 73 (11): 1765–82.\
(4) Orchard, S., Hermjakob, H., The HUPO proteomics standards initiative–easing com-munication and minimizing data loss in a changing world. Brief. Bioinformatics 2008,9, 166–173.\
(5) Deutsch, E., mzML: A single, unifying data format for mass spectrometer output. Proteomics 2008, 8: 2776-2777.
