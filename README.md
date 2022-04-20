# MITO-Sheets

# Installing Mito
## How to get a Mito sheet rendering on your own JupyterLab

### First open a new terminal or command prompt. Then, download the Mito installer:

python -m pip install mitoinstaller

### Then, run the installer. This command may take a few moments to run:

python -m mitoinstaller install


### To create a Mitosheet, open a new or existing JupyterLab notebook. The common command to start JupyterLab is 

### python -m jupyter lab. 

If you don't know how to create a JupyterLab notebook

### Once you've created a notebook, copy and paste the code below into a Jupyter code cell.

import mitosheet
mitosheet.sheet()

### Then run the Mitosheet generating code by clicking on the code cell that contains it and pressing Shift + Enter.


## Passing Dataframes to Mito

Mito displays any dataframe that is passed directly to a mitosheet.sheet(df1, df2). To see an example of displaying a dataframe in a Mitosheet, copy and run the code below in a JupyterLab cell:

# import Python packages
import mitosheet
import pandas as pd

# create some simple data to display

train_stations = pd.DataFrame({'Zip': [21001, 97321, 49224, 87102, 24910, 22301], 'City': ['Aberdeen', 'Albany', 'Albion', 'Albuquerque', 'Alderson', 'Alexandria'], 'State': ['MD', 'OR', 'MI', 'NM', 'WV', 'VA'], 'Ticket_Office': ['N', 'Y', 'N', 'Y', 'N', 'Y']})
demographics = pd.DataFrame({'Zip': [21001, 97321, 49224, 87102, 24910, 22301], 'Median_Income': [53979.0, 112924.0, 37556.0, 28388.0, 30914.0, 54087.0], 'Mean_Income': [66169.0, 147076.0, 50371.0, 39529.0, 40028.0, 64068.0], 'Pop': [18974.0, 11162.0, 14900.0, 22204.0, 5383.0, 19504.0]})


mitosheet.sheet(train_stations, demographics)
