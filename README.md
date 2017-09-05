# Ocean Navigator General use

The Ocean Navigator is a tool to make accessing detailed ocean scientific research data more accessible.
While it's main target users are scientists, the tool does not require a science background to use.
most of the data is predictive, however, using the Class4 and the Drifters exact data can be seen.

Please note: The Ocean Navigator is still in active development in order to both expand its functionality and to fix known bugs. A summery of some of the known bugs that may have an impact on the data displayed in the Ocean Navigator can be seen below in the [known bugs](#known-bugs) section for, more details see the [full list](https://github.com/DFO-Ocean-Navigator/Ocean-Data-Map-Project/issues) on GitHub. 

## Settings Left bar

On the Left side of the tool, there are several drop down lists, the details of each and their purpose are detailed below
![map setting (left bar)](https://2.bp.blogspot.com/-CQJ0IiAHMaA/WV-UtIGtC6I/AAAAAAAAAAk/x_bjzwPy0u8gNkRFjRTJSG-aCabasY2qACLcBGAs/s1600/left_bar_settings.png)
map settings left the bar

### Projection

the global projection will be the view that most users will need, however for users that want to view the north or south poles those options exist in the drop down here.

### Basemap

This drop down allows the user to select the type of underlying map. This will affect how the land appears.

using the "Show Bathymetry Contours" check box Bathymetry lines in the ocean can be turned on or off.

### Dataset

this allows for a selection of the different data sets, some datasets contain different types of data and some have recorded the same data in different ways.

### Variable

this dropdown includes a list of what can be viewed on the map. It includes options such as temperature, ice thickness, salinity and water vocality.
Each data set has its own set of available Variables and most are not available to all the datasets.
It may take a few tries to find the data set that has the variables you are looking for in it.

### Depth

Changing this values allows for values below the surface of the ocean to be viewed. If this value is 0 it is the surface value. higher values are deeper in the ocean. The default is surface.

### Time

This field allows data to be viewed for the past. any dates in the past that are included in the data set can be viewed. some data sets go back further than others.

### Variable Range

The Variable Range changes how the colors on the map will appear, making the range narrow will show a more produced difference in the range selected.
anything outside the selected range will appear as the max or min color depending on if it is above or below the selected range respectively

pressing the auto button will change the range such that for the current view the min and max values on the map will become the min and max values on the scale respectively.
this scale will remain the same as the view is changed. pressing the Default button will return the scale back to its default values range for that variable.


## Top Bar
![map setting top bar](https://3.bp.blogspot.com/-HciIgD7LLN4/WV-UtceUi2I/AAAAAAAAAAs/2FrkOU5xH1IaRNoiFd2viKzcf61tKi0VQCLcBGAs/s1600/top_bar_settings.png)

### Drawing 
The top bar has serval tools that allow for more detailed analyses of the selected data.
the point, line, and area options have some predefined selections that can be chosen
in addition, in the drop-down lists there is also the option to upload a CSV of points or a to draw your own. you can also draw your own line/shape simply by clicking on the respective button.
when drawing a shape or line search click will add a new point in the line for a shape you need to link it back to the start to finish it or you can double
click to end on that point which will end the shape by linking that point to the start. Clicking on the same point twice in a row is also how to end drawing a line.

after the selection has been made a new window will open showing the section of map selected.

#### CSV format

When uploading a CSV file (Comma Separated Value) there must be a header line. This header must contain the terms "latitude" and "longitude" to indicate which columns hold this information. These columns will then be used for plotting the points/lines/Areas. If there are extra columns they will be ignored. an example file can be seen [here](https://github.com/DFO-Ocean-Navigator/Ocean-Data-Map-Project/wiki/example-CSV).

### Class 4
'Class 4' is an ocean data standard of directly observed data. The purpose of this standard format is so that predictive models can be compared against the true observe data at a particulate location. this can aid in the validations of predictive models and helps predictive models reduce their discrepancies.
more information about class 4 can be found in the links below

[Class 4 presentation slides](https://www.godae.org/~godae-data/OceanView/Events/MEAP-TT-workshop-June-2015/4.2-MEtrics_MEAPP.pdf)

[Class 4 Article](http://www.tandfonline.com/doi/full/10.1080/1755876X.2015.1022330)

### Drifters

Selecting the "drifters" drop down list will provide the option to either show a category of drifters or to select just one drifter. once selected the drifter(s) will appear on the main map, from there more information can be seen about the drifter by clicking on its path. this will open a popup window about the drifter. 

### Plot
This button is grayed out until the line or point functions have been used.
if the Point or line functions are used and the pop-up window has been closed pressing the Plot button will reopen that window.
Pressing on the line or dot will also reopen the window.

### Rest map/Refresh

This cycle arrow button simply clears the map of any points, lines or areas that have been selected. It does not reset other settings. To reset everything uses the browsers refresh button.

## keyboard shortcuts and Other

There are 2 keyboard keys that will provide extra features. These are _shift_ and _ctrl_ their function depends on the action that is being performed at the time.  Continue reading for more details. 
 

### plotting multiple points 

When there have been multiple points displayed on the map (ex from an uploaded csv file), multiple can be selected at the same time

#### Point by point
This can be done by pressing shift and then clicking on the point(s) you would like to view. After selecting all the points, press plot to have them all drawn on the same graph. 

#### Selection box
Pressing and holding Ctrl will allow the user to draw a selection box to select multiple points at the same time. After selecting the desired points, press plot to have them all drawn on the same graph. 

### Drawing curved lines
After selecting the option to draw a line or area from the tool bar, a curved line can be drawn by pressing and holding shift while drawing the line. 

### Quick zoom
Pressing and holding shift will allow for an area to selected for a quick zoom. 


## Technical Details

Ocean Navigator is a Data Visualization tool that enables users to discover and view 3D ocean model output quickly and easily.

The ocean model output is stored in [NetCDF](https://en.wikipedia.org/wiki/NetCDF) files. These files are self-describing and contain the 2D or 3D model output for one or more timesteps and one or more variables.

To facilitate reading all these files, we make use of a server called [THREDDS Data Server](http://www.unidata.ucar.edu/software/thredds/current/tds/). THREDDS aggregates all the NetCDF files and allows users to query subsets of the files.

### Known Bugs

 Below is a summary of some of the known bugs in this program that are being worked on. More details and a [full list of bugs](https://github.com/DFO-Ocean-Navigator/Ocean-Data-Map-Project/issues) can be found on our [GitHub page](https://github.com/DFO-Ocean-Navigator/Ocean-Data-Map-Project). 

 * 1) [resolution problem](https://github.com/DFO-Ocean-Navigator/Ocean-Data-Map-Project/issues/7). In areas where there is a high gradient in the data, there can sometimes be a problem in the color map in the form of blotches of color being rendered. This *will* effect the data values viewed. This is a byproduct of the type of interpolation that is being done to generate a continuous map from a series of data points.
 
 * 2) [velocity plot](https://github.com/DFO-Ocean-Navigator/Ocean-Data-Map-Project/issues/53) The velocities that are displayed north of 40N on the map are known to be displayed in the wrong directions. This is a result of misrendering the information from a tripolar grid to the grid used by the ocean navigator.
 
 * 3) [Southern Hemisphere misaligned](https://github.com/DFO-Ocean-Navigator/Ocean-Data-Map-Project/issues/4) When zoomed to the max zoom level in the Southern Hemisphere the data is not allined with the dislayed view (it is offset by about 70 Km). At the zoom levels that are not the max level this is not an issue.   

## Citations

Hernandez, F. "List of internal metrics for the MERSEA GODAE global ocean: specification for implementation. MERSEA IP report MERSEA-WP05-MERCA-STR-0015-01C. doc." (2007).
