
<span style="color:green"><h1>UCLA, Fall 2024 </span> <span style="color:yellow"> ****</h1></span>
<span style="color:blue"><h2>Professor Abeer Alwan, alwan@ee.ucla.edu</span> <span style="color:yellow"> ****</h2></span>
<span style="color:blue"><h3>Dept. of Electrical Engineering EE214A: Digital Speech Processing</span> <span style="color:yellow"> ****</span>


# <span style="color:green">Guide to setup local environment</span> <span style="color:yellow"> ****</h1></span>

Here's a step-by-step guide to creating a Python runtime environment in Visual Studio Code (VS Code) to run a Jupyter notebook:

### Step 1: Install Python
Ensure that Python is installed on your system. You can download it from [python.org](https://www.python.org/).

<span style="color:orange"> Note: Instruction on "https://docs.python-guide.org/starting/install3/osx/" site can be a good way to install python. </span>

### Step 2: Install Visual Studio Code
Download and install Visual Studio Code from [code.visualstudio.com](https://code.visualstudio.com/).

### Step 3: Install Required Extensions
Open Visual Studio Code and install the following extensions:
1. **Python** extension by Microsoft
2. **Jupyter** extension by Microsoft

You can find these extensions in the Extensions view (Ctrl+Shift+X).

### Step 4: Set Up a Virtual Environment
1. **Open a terminal** in Visual Studio Code (View > Terminal or `Ctrl+``).
2. **Navigate to your project directory**:
   ```sh
   cd your_project_directory
   ```
3. **Create a virtual environment**:
   ```sh
   python3 -m venv .uclavenv
   ```
   Here, `myenv` is the name of the virtual environment.

4. **Activate the virtual environment**:
   - On Windows:
     ```sh
     myenv\Scripts\activate
     ```
   - On macOS/Linux:
     ```sh
     source myenv/bin/activate
     ```

### Step 5: Install Jupyter and Other Dependencies
Once the virtual environment is activated, install Jupyter and any other packages you need for your project:
```sh
pip install jupyter pandas numpy matplotlib
```

### Step 6: Create and Open a Jupyter Notebook
1. **Create a new Jupyter notebook**:
   ```sh
   jupyter notebook
   ```
   This command will open the Jupyter notebook interface in your web browser.

2. **Create a new notebook** and save it in your project directory.

### Step 7: Configure VS Code to Use Your Virtual Environment
1. **Open your project directory** in Visual Studio Code.
2. **Open the Command Palette** (Ctrl+Shift+P) and type `Python: Select Interpreter`.
3. **Select the interpreter** from your virtual environment (`myenv`).

### Step 8: Open Jupyter Notebook in VS Code
1. **Open the Jupyter notebook** file you created (`.ipynb`) in Visual Studio Code.
2. **Run your cells** directly in VS Code.

### Summary Script
Here’s a summary script for setting up the environment (run these commands in the terminal):

```sh
# Navigate to your project directory
cd your_project_directory

# Create and activate the virtual environment
python -m venv myenv
source myenv/bin/activate  # use `myenv\Scripts\activate` on Windows

# Install Jupyter and other dependencies
pip install jupyter pandas numpy matplotlib

# Start Jupyter notebook
jupyter notebook
```

By following these steps, you should be able to set up and run a Jupyter notebook with Python code in Visual Studio Code. 