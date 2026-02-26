# PS-NE-329
PS/NE329 Experimental Psychology: Cognitive Neuroscience -- A practical introduction to EEG experiments and data analysis

This course teaches EEG Data Analysis with Python, Jupyter, and MNE

## Getting Started

### Analysis Environment
In this course, we'll use Jupyter Notebooks as a convenient way to run Python code. The main toolkit in Python we use for EEG data analysis is MNE. The following section provides a quick and easy method to get set up. For advanced programmers I recommend managing local environments using `uv`.

### Installing Jupyter on you own computer
The simplest way of using Jupyter is to install and run it as a desktop application. You can find installers for all major operating systems [here](https://github.com/jupyterlab/jupyterlab-desktop?tab=readme-ov-file#installation).

#### Setting up Python
Jupyter needs Python to execute your code. The first time you start the dekstop app, it will ask you to download it. Simply click the prompt at the bottom of the window:
![[attachments/screenshot.png]]

The installation takes a minute. When it is finished, you can click on the "Open" icon and navigate to the folder for your project. Next you will see the option to Launch different environments - select 'Notebook' > 'Python 3 (ipykernel)' to create a new notebook.

### Using Jupyter in the Computer Pool

A different version of Jupyter is pre-installed on the BU Computer Pool machines. Search the Window Menu for "Jupyter Notebook" and run the link. This will first open a console window (which you can ignore) and then navigate a browser window to a local address for the Jupyter server. You may choose to switch the Jupyter interface to the more functional "Jupyter Lab" in the "View" menu. Python is already provided in this instance, but you will still need to follwoing step to install MNE.

### Installing MNE
Before you can run any interesting code, you need to install the correct libraries for analyzing EEG data in Python. Simply paste the following line in a cell in your new notebook, and run it by hitting 'Shift + Enter'. A bunch of messages will pass by and once Jupyter is done you should have everything you need (and you never need to run the command again).

```python
%pip install mne-icalabel mne-connectivity h5io --force-reinstall --no-cache-dir
```

The asterisk to the left of your command indicates that the computer is processing your request. Once it turns into a number, you can restart the Kernel in the 'Kernel' menu. To confirm success, try running `import mne`.

## Data Analysis

