 Julia2018TouchUI
==================
Touch UI for Julia 2018

## Development Requiements:

[ A simple getting started guide](https://nikolak.com/pyqt-qt-designer-getting-started/)


1. PyQt4, Qt Designer and other Qt related dependencies from Development Repository (https://github.com/FracktalWorks/DevelopmentTools)
3. Websocket client ( pip install websocket-client )
4. other dependencies that "Main.py" needs (see it's headers)

The MainGUI.py file is generated from the mainGUI_pro_single_abl.ui file using
```pyuic4 .\mainGUI_pro_single_abl.ui -o .\mainGUI_pro_single_abl.py```



## Running/Executing:

**Octoprint needs to be running in order for the Touch UI to work, since it uses octoprint's api functionality**

1. point the "ip"  and "apiKey" to where Octoprint is living. Point it to the local host in case it is running on the same system
2. in case of running it on anything other than a raspberry pi, disable the raspberry pi option




## To Install:

1. Install Octoprint:
..* git clone into root directory of Raspberry Pi https://github.com/FracktalWorks/Julia2018Octoprint.git
..* Change into the OctoPrint folder: cd Julia2018Octoprint
..* Create a user-owned virtual environment therein: virtualenv venv
..* Install OctoPrint into that virtual environment: ./venv/bin/python setup.py install
..* Follow other instructions for automatic startup

2. Install TouchUI into Octoprint:
..*