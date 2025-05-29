#Dual-Input-HSN-Validator

This notebook implements a dual‑input neural network using TensorFlow/Keras that feeds the HSN code (character‑level) into a bidirectional LSTM to learn valid patterns and catch subtle typos.


A video walkthrough of this repository is available as a release asset under the Dual_Input_HSN_VideoExp tag. You can download or stream it here:

▶️ https://github.com/SunnyUI-cyberhead/Dual-Input-HSN-Validator/releases/download/Dual-Input-HSN-Validator/HSN_Code_Validator_VideoExp.mp4 (50 MB)


****Before running the code, we first download or copy the Excel workbook HSN_SAC.xlsx (containing the HSN_MSTR and SAC_MSTR sheets) into a data/ folder at the root of this repository. Next, we update the DATA_PATH variable in both our notebook (notebooks/Dual_Input_HSN_Validator.ipynb) and our module (src/validator.py) to point to "data/HSN_SAC.xlsx", and we verify that the SHEET_NAMES mapping matches our sheet names. Once we’ve directed the code to data/HSN_SAC.xlsx, the data-loading routines will automatically ingest our master lists and the dual-input validation pipeline will run seamlessly.

Usage

With the data file in place and DATA_PATH set:

Notebook: Open Dual_Input_HSN_Validator_NB.ipynb in Jupyter or VS Code and run all cells.

Script: Import and call the validation functions in dual_input_hsn_validator_src.py from your own Python code.

The data-loading routines will read the master lists and the dual-input validation pipeline will execute automatically.


License

MIT © SunnyUI-cyberhead

