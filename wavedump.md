# Wavedump
## Configuration file
The digitiser uses the config file ending in "_x1742.txt"
The important things that may need changed are:
- signal sign (positive or negative)
- enable the group/channel you want
  - note: if you are using > 8 channels it will only display the first 8 in plotting (it will still write the rest)
  - if you want to visualise groups 1+, disable group 0, etc..

## Recording Data
1. Navigate to the folder you want to record the data to (Should be a work disk or scratch disk as we will write big data files)
2. from the np-bbox1 machine (ssh or locally) run the wavedump software.
3. Press "W" to enable continuous writing mode
4. Press "P" to show liveplots
5. Start and stop the data aquisition with "s"
6. More commands can be viewed by pressing "space"
