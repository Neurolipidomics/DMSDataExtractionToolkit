# DMS Data Extraction Toolkit
Field asymmetric (differential) ion mobility spectrometry (FAIMS/DMS) data are generated using user-specific proprietary platforms with their own file formats.  For example, experiments generated on a SCIEX® SelexIon instrument will produce .wiff and .wiffscan datafiles. To format [iDMS](https://github.com/Neurolipidomics/iDMS) input, users must manually produce their sample input files, or they can first convert their proprietary files to JCamp (.jdx) or mzML files and then use the DMS Data Extraction Toolkit to batch extract their iDMS .csv files.

# Setup
DMS Data Extraction Toolkit was developed in Python 3.12.10 and provided as Jupyter notebooks and Python scripts. Manuals assisting users to set up their computers to run DMS Data Extraction Toolkit successfully are available in either folder.

# Naming convention for input files
Datafile input for DMS Data Extraction Toolkit must be in this format for a successful conversion.

[text]_[SV value]_[text].mzml (or .jdx)

For example: SV_2000_Pos.mzml

# Bug Report:
For bug report, please contact Dr. Steffany Bennett at SteffanyAnn.Bennett@uottawa.ca and Thao Nguyen-Tran at tnguy32@uottawa.ca. Please also send an example .jdx or .mzML file that did not run successfully through the DMS Data Extraction Toolkit.

# Citing
Nguyen-Tran, T., Shi, XX., Hashimoto-Roth, E., Organ, M.G., Lavallée-Adam, M., Perkins, T. J. & Bennett, S.A.L. (2026). Intelligent differential ion mobility spectrometry (iDMS) for lipidomics: A machine learning algorithm that predicts the optimal space -resolved ion mobility parameters for isomeric glycosphingolipids.

