# Script: Translation Vendor Database

## The repository
This repository has been created by Elmo Geeraerts for the final assignment of an introductory class on python.

The repository contains:
- The `README.md` file which describes the repository and illustrates how to use the code as a module and by running the script;
- The `tutorial.md` and `tutorial.ipynb` files which show how to actually use the code and the different functionalities;
- The `example.json` file which allows the user to test out the code;
- The `vendor_data.py` file, i.e. the actual python script that can be run or imported as a module.

## Installation and usage

### As a module
Clone this repository with the following git command in the console (or download the ZIP file via GitHub):

```sh
git clone https://github.com/ElmoGeeraerts/intro_machine_learning_using_python.git
```

You can import the script as a module by adding the repository to your path in a Python script or interactive notebook and then calling `import`.

```python
import sys
sys.path.append('/path/to/intro_machine_learning_using_python')
import vendor_data as vd
```

Check out `tutorial.md` to see an example of the different functionalities of the script!

### Running the script
You can also run the script directly with the following code in a console:

```sh
python vendor_data.py <example.json>
```

Or in Jupyter notebook with:

```python
%run vendor_data.py <example.json>
```

In both cases `example.json` stands for the `filename` argument that the script needs. You can use [the file in this repository](example.json) or a similar file of yours. Find more information on how this script works with:

```sh
python vendor_data.py --help
```

## What this script CAN do

This script is supposed to help translation project managers with keeping a clear overview of the vendors working on the a particular project.
The script allows the project manager to:
1. Easily create an excel file with the project name and the source language as filename;
2. Write the following data to the excel file: the target language and the translator's name, e-mail, word rate, preferred CAT tool and the status of the translator;
3. Modify the following data for the vendors already in the excel file: e-mail, word rate, preferred CAT tool and status.
The main advantage of this script is that it limits the posibilities of CAT tools and statuses and that it validates e-mail and word rate (betw. 0.01 and 0.15). This prevents the excel file from becoming messy when different people are working on the project.

## What this script CANNOT do
There are limits to this script that - with more practice, knowledge and time - might be resolved in the form of new functionalities.
With this script you CANNOT:
- Look up specific vendors;
- Joining multiple excel files in the excel file created by this code.
