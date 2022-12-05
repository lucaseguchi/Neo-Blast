# Neo-Blast
# Software Neo Blast for Blast Design and Environmental Impacts Assessments

This is a small Python3 application that moves files whose names match a user input regular expression. The source and destination directories are specified by the user and can not be remote directories. As long as the program is running, the code checks if there are new valid files in the source directory based on a timer and continuously shows plots and statistics regarding the files that were moved. The source and destination directories must exist and be writable for the program to run.

This program was written and tested in a Linux machine with Python 3.8.

<img src="https://ibb.co/S61xcRn" alt="Software-Neo-Blast" width="700"/>

## Dependencies

 - [PyQt5](https://pypi.org/project/PyQt5/)

## Installation & Usage

After the installation of the dependencies, download (or clone) this repository and extract all files. To run the program, switch to the extracted folder and execute the main script.

```bash
$ cd moving_files
$ python3 Neo Blast.py
```

Finally, write down the regular expression, source and output directories and set the timer. Click "Start" when ready and the program will start moving the files (if there are any). The progress can be tracked with the statistics and plots boxes or the status bar.

**Caution**: Closing/quitting the program while it is running may corrupt files.

## Menu & Buttons
The menu is simple and allows the user to change the window style, clear all data generated during the last run of the program, exit and show program information.

In the main window there are two buttons: "Run" and "Clear". The "Run" button checks if the inputs are valid: the regular expression must compile and the source/destination directories exist and are writable. The "Clear" button clears all inputs and sets the timer to the default value.
