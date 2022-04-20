# MITO-Sheets

# Installing Mito
## How to get a Mito sheet rendering on your own JupyterLab

### First open a new terminal or command prompt. Then, download the Mito installer:

python -m pip install mitoinstaller

### Then, run the installer. This command may take a few moments to run:

python -m mitoinstaller install


### To create a Mitosheet, open a new or existing JupyterLab notebook. The common command to start JupyterLab is python -m jupyter lab. If you don't know how to create a JupyterLab notebook

### Once you've created a notebook, copy and paste the code below into a Jupyter code cell.

import mitosheet
mitosheet.sheet()

### Then run the Mitosheet generating code by clicking on the code cell that contains it and pressing Shift + Enter.
