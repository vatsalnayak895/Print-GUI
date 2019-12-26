# Print-GUI
This was a project done during my first internship experience in the United States of America, this was an adhoc project for the packaging department to help them print labels for labeling the manufacturing units.
The main aim of the project was to reduce the dependency of employee working in packaging on the IT department and overall time savings in terms of time spend in communication and involvement of multiple department for a single unit task of printing packaging labels. 
The GUI was developed considering all the aspects of packaging and the user comfort of printing the labels, deployement of the GUI for the user had multiple preliminary stages.
## Requirement Gathering: 
This phase helped understad the use case of the GUI and how it would benifit the company and the employees. The entire manufacturing process was understood, differnt jobs resulting post manufacturing were noted.
## Design Phase:
Basic design for the GUI was developed on paper. The purpose of the GUI was explained to the packaging department and their views on the GUI were considered.
## Development Phase:
The development was python based, PyQt5 was the main package used for the GUI development, it was used to develop the structure and the functionalities of the GUI. Other packages like sys, os, shutil were used to manipulate the output file. The development started with created the structure of GUI and then appending the logic to it generate the output text file.
The output file generated was then moved from local machine to the print server from where the printer would read the text file and execute the prints in the order they are mentioned in the output file.
## Testing Phase:
GUI was tested on various usecases that were discussed during the requirement gathering phase. The employees were given the GUI to use and asked to review it according to their expectation and required changes were made.
## Production Phase:
Python was installed on the server and all the required packages were installed on the server. The GUI was implemented on the server and a shortcut of the triggering bat file was moved to the Desktop of each user instance so that the useres can access the GUI from their local machines for printing the labels from their end.


# Code:


import shutil
import sys
from PyQt5.QtWidgets import * #QApplication, QWidget, QInputDialog, QLineEdit, QLabel , QPushButton, QPlainTextEdit, QTextEdit 
from PyQt5.QtGui import *
from PyQt5 import QtWidgets
from PyQt5 import QtGui
from PyQt5 import QtCore
import datetime
import os


