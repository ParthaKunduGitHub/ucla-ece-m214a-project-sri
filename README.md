Here’s the organized and formatted version of your text to include in a README file:

---

# Project: Noise Robust Speaker Region Identification

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Prerequisites](#prerequisites)
3. [Getting Started](#getting-started)
4. [Running the Notebooks](#running-the-notebooks)
5. [Formatting of the Notebooks](#formatting-of-the-notebooks)
6. [Additional Information](#additional-information)

---

## Project Overview
This project focuses on identifying the region of a speaker's origin using noise-robust techniques.

---

## Prerequisites
- Access to the Google Drive containing the data or the capability to edit each notebook with a controlled Google Drive path.
- The original datasets should be loaded in the designated folder.

---

## Getting Started

1. **Sign in to Google Account**:
   - Ensure you have access to the proper drive path.
   - To allow Google Colab notebooks to find the drive, ensure the path appears the same for everyone running the notebook.
   - If the data folder is shared, add a shortcut to your drive ensuring the path matches the code.

2. **Open Google Colab**:
   - Ensure you're signed in with the correct Google account.
   - Link Google Colab to GitHub: Go to File > New Notebook > GitHub tab. Authorize your GitHub account.

3. **Pull Code from GitHub**:
   - Go to GitHub User Avatar > Settings > Developer Settings > Personal Access Tokens. Generate a new token with full repo privileges.
   - In Google Colab, click on the key icon in the left bar. Add two secrets:
     - `gh_username`: Your GitHub username.
     - `gh_pat`: The generated GitHub token.
   - NEVER log these variables.

---

## Running the Notebooks

1. **Run Notebooks**:
   - Follow the steps above to ensure each notebook runs smoothly.
   - On the first run, grant access to Google Drive and GitHub secrets.
   
2. **Manage Data**:
   - The `GoogleDriveDataIO` utility class will load and save data to the specified path. Overwrite existing results as needed, or point to a different path to avoid overwriting.
   - For long-running notebooks, consider saving the result and short-circuiting the corresponding cell.

---

## Formatting of the Notebooks

**"F24_ECE_M214A_Final_Project.ipynb"** is the main Jupyter notebook and is formatted as follows:

1. **Structure**:
   - The notebook is divided into four major parts, each with multiple sections.

2. **Task-Specific Cells**:
   - Each cell performs specific tasks and can be skipped by enabling the "%%skip" tag at the beginning.

3. **Directory Paths**:
   - Defined in section 2.c. Adjust paths as per the executing environment before running the notebook.

4. **Feature Extraction Algorithms**:
   - Thirteen different types of feature extraction algorithms are implemented (section 3.a).

5. **Feature Extraction Execution**:
   - Called from section 3.b. The notebook is configured to run the best combination based on the experiment (ComParE + PNCC + PLP + Wav2Vec2 + LPC_26 + MEL).
   - Place the features with CSV files in the "dataFrame/features" folder. Uncomment the "%%skip" tag in section 3.b to regenerate CSV files if needed.
   - Ensure the file names match those used in section 4.a when placing new CSV files.

6. **Training and Accuracy**:
   - Section 4.c is used for training the model and producing accuracy results.
   - Configure the `n_dataframes` variable with index numbers of dataframe combinations (from 4.b) based on execution requirements.

---

## Additional Information

### Package_info
- Versoions and license information of used packages/libraries can be found in "package_info.txt" file located in root directory. 

### Troubleshooting
- **Common Issues**: TBD
- **Support**: Contact - Project Team

### Contribution Guidelines
- Fork the repository.
- Create a new branch (`git checkout -b feature-branch`).
- Commit your changes (`git commit -am 'Add new feature'`).
- Push to the branch (`git push origin feature-branch`).
- Open a Pull Request.

### License
- TBD