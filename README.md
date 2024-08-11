# Tutorial for LSCE ALICE -- a simple and versatile alignment interface for icecores

Tutorial for ALICE with example data.

## Installation

See instructions on the [pypi project page](https://pypi.org/project/lscealice/)

## Creating a new alignment file from data
Select `create alignment file` in the `File` menu and follow the steps in the pop up window.

- Your icecore data must be formated in an `.xlsx` or `.ods` format, with each tab corresponding to an icecore, first column for depth, and other columns for isotopologue or chemical species.

- Note that multiple data files may be selected, allowing you to work with data at different resolution for the same core (e.g. discrete and CFA measurements).

## Using the interface

### Alignment

- Add tiepoints: <kbd> left click </kbd>  on the plot adds tiepoints successively on the two curves
- Delete tiepoints: Hovering over the plot will highlight the closest tiepoint. <kbd> Right click </kbd> on a highlighted pair of points to delete it.

- You can use the native `zoom` and `pan` widgets of matplotlib to focus on some areas of the curves to align.

- <kbd> Left arrow</kbd> and <kbd> Right arrow </kbd> lets you navigate through cores.
- <kbd> Up arrow </kbd> and <kbd> Down arrow </kbd> lets you cycle through species
- Some species have default keys assigned to them: <kbd> S </kbd> Sulate, <kbd>w</kbd> MSA, <kbd> o </kbd>  $`\delta^{18}`$ O,...


### Preview: 
- The aligned data series will be displayed on top of the reference data series in the bottom part of the interface.

## Working with `.pkl` files.
### Store your alignment
Curently, changes are automatically saved to the `.pkl` file.
### Opening an alignment file
Click the `File` menu then `Open alignment file` and select a `.pkl` file to resume working on your alignment.

## Exporting the result
Click the `File` menu then `Export to .csv` and follow the instructions in the pop up window to save the aligned cores to a .csv file for later data analysis of the aligned data in Jupyter Notebook or Matlab.


Have fun!🐧
