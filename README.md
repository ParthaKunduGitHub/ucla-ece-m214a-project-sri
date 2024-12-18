# ucla-ece-m214a-project-sri
Project : Noise Robust Speaker Region Identification 

## Prerequisites

You will need access to the data Google Drive or each notebook will need to be edited with a Google Drive path that you control and all data will need to be rebuilt. To start the folder should have the original datasets loaded. 

## Getting started

1. Sign into the Google account that has access to the proper drive path. In order for the Google Colab notebooks to find the drive it must appear in the same place in the drive of everyone who attempts to run the notebook, or you must change the path in the notebook before running it. If the data folder has been shared with you, go to Shared with me, right click on the folder, and add a shorcut to your drive. Make sure that the path in your drive is the same as the path in the code, this is critical.
2. Open Google Colab, ensure you are still in the Google account with access to the data. We need to link Google Colab to GitHub. Go to File > New Notebook. In the popup window there should be a tab that says GitHub. Click on that and go through the process of authorizing your GitHub account (that has access to this repository) by logging in.
3. The above step allows us to open notebooks from GitHub and commit back to the repository but it doesn't allow us to pull the code from the repository which is where the reusable utilities are located. To do this, go to your GitHub User Avatar > Settings > Developer Settings (all the way at the bottom) > Personal Access Tokens > Tokens (classic). Generate a new token and make sure to give it full repo privileges. Copy the token when it is shown (this is your only chance!) and save it somewhere safe. Go back to Google Colab and on the left bar click on the key icon. Add two secrets. First secret is named gh_username and should be your GitHub username. Second secret is named gh_pat and should be the token you just got from GitHub. When you run a notebook it will pull these variables into the Python code and pull down the remainder of the code. NEVER LOG THESE VARIABLES.

## Running the notebooks
If you followed the above steps each notebook should run without problem. On the first run of a notebook it will ask for access to your Google Drive and popup a login window and will ask for access to the secrets you put your GitHub information in. Allow them all. Note that the utility class GoogleDriveDataIO will automatically load and save data to the specified Google Drive path and will overwrite results that already exist there. If you would like to avoid that, point the class to a different path that it can save the results to. For longer running notebooks or commands consider running them only once and then short circuiting that cell by loading in the result instead. Please be careful to not overwrite good data when running the cells. 

<!-- Note: If it is plan to run this code in colab, please make sure to run the first three cells which are under "Execute only for Google Colab Environment" section of the notebooks and skipp the cells under "Execute only for Laptop Environment" section. If you are planning to execute the in laptop, please make sure to skipp "Execute only for Google Colab Environment" section and execute the cells under "Execute only for Laptop Environment" section of the notebook.  -->

