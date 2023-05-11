
The Ocean Navigator is a visualization application for digital ocean information that was developed to make numerical ocean environment prediction estimates and in-situ ocean observation available to end users. It includes a number of different variables such as temperature and ocean currents. The tool is designed for any user; be it a researcher writing a technical paper, or a hobbyist interested in the oceans.

# Ocean Navigator Overview


![Ocean Navigator Overview](screenshots/overview.png "Ocean Navigator Overview")

### 1. Main Map

The main map is the most prominent way to visualize oceangraphic forecast models in the Ocean Navigator. The default view is centered on the North-West Atlantic but users can pan over map clicking and dragging at any point. Users can also zoom in or out using their mouse wheel, laptop touchpad, or by using the zoom buttons present in the [Additional Options](#5-additional-options) area. 

The main map is highly customizeable and users are given the ability to change the map projection, basemap layers, bathymetry, and more. See [Changing Map Settings](#changing-map-settings-) for more details.

### 2. Dataset Selection Panel

![Dataset Selection Panel](screenshots/dataset_selector.png "Dataset Selection Panel")

The dataset selection panel allows users to view datasets from the Ocean Navigator's data catalog on the main map. There are several menus that users can use to modify the data presented. Once the user has selected a data product and the relevant parameters they must click the _Go_ button to display the data on the main map. The data set selection menus are described in detail below. 

1. Dataset Selector

   ![Dataset Dropdown Menu](screenshots/dataset_dropdown.png "Dataset Dropdown Menu")

   The dataset drop down allows users to select data from one of the many forecast models available in the Ocean Navigator. Within the dataset dropdown menu data is first grouped by forecast then other relevant details such as dimensionality, time range, and climatologies. 

2. Variable Selector

   Allows users to choose a varaible from the currently selected dataset.

3. Quiver Selector

   Users can display vector variables as quiver arrows drawn over the global map view by selecting a variable from the quiver dropdown menu. 

   ![Quiver Arrows](screenshots/quiver_arrows.png "Quiver Arrows")

4. Depth Selector

   This dropdown menu allows the user to change the depth level of the currently selected dataset. The highest level is selected by default and the selector will not apear for two dimensional datasets.

5. Compare Datasets Switch

   This switch allows users to display two datasets simultaneous and make comparison line and area plots between the two. See [Comparing Datasets](#Comparing-Datasets) for more details.

6. Timestamp Slider
![Time Slider](screenshots/time_slider.png "Time Slider")

   Users can select the model forecast time on the main map using the _timestamp slider_. The currently selected time is indicated by the slider thumb <img src="screenshots/slider_thumb.png" width=20 height=20 />. 
   
   To select a new timestamp users can click on any tick along the timestamp slider or select an adjacent timestamp using the previous and next buttons located on each end of the slider <img src="screenshots/chevron.png" height=20 />.

   Due to size contraints the the timeslider only displays labels for major ticks at 00:00 and 12:00 for hourly datasets but a tooltip will appear over the minor ticks indicating their time. For larger datasets with more than 48 available timestamps the <img src="screenshots/double_chevron.png" height=20 /> buttons will cycle though groups of timestamps. 

7. Go Button

   The _Go Button_ is used to enact the changes that the user has made through the menus above. 

### 3. Data Scale Viewer

![Data Scale Viewer](screenshots/scale_viewer.png "Data Scale Viewer")

The Data Scale Viewer displays the colormap scale of the currenly displayed variable. Clicking on the data scale viewer will reveal the _Colormap Range_ selector. Here users can adjust the maximum and minimum values of the current colormap by entering new values or clicking the _Auto_ button which will scale the colormap to the data range within the area currently visible on the map. Clicking _Default_ will restore the original colormap range. 

### 4. Navigator Map Tools

#### Draw Point Coordinates <img src="screenshots/draw_button.png" width=35 height=35 />
Clicking this button enters drawing mode and the Navigator's drawing options are displayed. The drawing options provide buttons to change the plot type (point, line, and area), undo a point, clear the map, and plot the coordinates added by the user. Once points have been added to the map their locations can also be modified using the [Enter Point Coordinates window](#enter-point-coordinates). For more details on drawing coordinates and plotting see [Selecting Coordinates and Creating Plots with the _Draw Point Coordinates_ Tool](#selecting-coordinates-and-creating-plots-with-the-draw-point-coordinates-tool).

#### Enter Point Coordinates <img src="screenshots/enter_button.png" width=35 height=35 />
Selecting this option displays the _Enter Point Coordinates window_. This feature allows users to enter the exact location of points of interest and plot data at those locations. Users also have the option of importing point coordinates from a CSV file. Like the _Draw Point Coordinates_ tool users can select from a variety of plot types and plotting that data. Any points present on the map, whether they have been previous entered via this window, imported from a CSV, or drawn on the map, can be modified in this window. See [Selecting Coordinates and Creating Plots with the _Enter Point Coordinates_ Tool](#selecting-coordinates-and-creating-plots-with-the-enter-point-coordinates-tool) section for more information. 

#### Preset Features <img src="screenshots/preset_button.png" width=35 height=35 />
The Ocean Navigator also provides users with a number of preset points, line, and areas that may be of interest to users. Clicking on this button will present the user with a menu where they can select from a variety of points of interest which can added to the map. Once on the map any of these features can be plotted by clicking on them. Note that selecting any of these options will remove all other points of interest from the map. 

#### Observations <img src="screenshots/obs_button.png" width=35 height=35 />
The _Observations_ button allows users to access the Ocean Navigator's observations database. When clicked the Observation options which gives the user a number of options for selecting observations or displaying class4 data. For a more detailed descrition of these options see [Viewing Observation and Class4 Data](#viewing-observation-and-class4-data).

#### Plot <img src="screenshots/plot_button.png" width=35 height=35 />
The _Plot_ button behavior is dependent on the data displayed on the map. For user selected point, lines, or areas clicking this button will open the appropriate [plot window](#ocean-navigator-plot-windows). In the event that multiple points were selected the resulting plot will contain all of them. For preset features, observaitons, and class4 points clicking this button will open a plot window for the most resecntly selected feature. 

#### Reset Map <img src="screenshots/reset_button.png" width=35 height=35 />
As implied, the _Reset Map_ button removes all features from the map. 

#### Settings <img src="screenshots/settings_button.png" width=35 height=35 />
This button will open the [settings window](#changing-map-settings) where users can modify the main map. 

#### Info/Help <img src="screenshots/info-help_button.png" width=35 height=35 />
Clicking this button opens the _Info/Help_ window where users can find dataset metadata, variable definitions, and help documents such as this one.  

### 5. Additional Options

![Additional Options](screenshots/additional_options.png "Additional Options")

1. Get link Button

   This button opens the _Share Link_ window. Here, users can generate a link to the current state of the Ocean Navigator and share it with others. When accessing the application through this link the current dataset options will be restored.

2. Language Selector

   Allows users to toggle between English and French

3. Cursor Coordinates

   Displays the current latitude/longitude cooridnates of the mouse cursor.
  
4. Zoom Buttons

   These buttons can be used to change the zoom level of the main map.

# Ocean Navigator Plot Windows

## Point Window

## Line Window

## Area Window

## Observation

## Class4

# Using the Ocean Navigator

## Navigating Data Displayed on the _Main Map_

## Selecting Coordinates and Creating Plots with the _Draw Point Coordinates_ Tool

![Drawing Options](screenshots/drawing_tools.png "Drawing Options")

![Points, Line, and Area](screenshots/point_line_area.png "Points, Line, and Area")

## Selecting Coordinates and Creating Plots with the _Enter Point Coordinates_ Tool <img src="screenshots/enter_button.png" width=35 height=35 />

![Enter Point Coordinates Window](screenshots/enter_coords_window.png "Enter Point Coordinates Window") 

![Add POint Coordinates](screenshots/add_coords.png "Add Point Coordinates")

## Creating Plots via the _Preset Features_ Menu <img src="screenshots/preset_features_button.png" width=35 height=35 />

![Preset Features Window](screenshots/preset_features_window.png "Preset Features Window") 

## Viewing Observation and Class4 Data <img src="screenshots/obs_button.png" width=35 height=35 />

![Observation Options](screenshots/obs_tools.png "Observation Options")

![Observation Window](screenshots/obs_window.png "Observation Window")

1.
2.
3.
4.
5.

![Class4 Selector](screenshots/class4_selector.png "Class4 Selector")

## Comparing Datasets

Checking the compare datasets box will bring up a side by side view of the data set. It will also provide settings in the left side bar for each view. Each view can be changed independently by setting the values in the corresponding settings box (ie left or right view). In addition, the plotting features, explained below in the Drawing section, will provide extra information when comparing datasets, most notably a difference plot will be shown when comparing variables that are similar.

![Compare Datasets Toggle](screenshots/compare_toggle.png "Compare Datasets Toggle")

![Comparing Datasets](screenshots/compare_map.png "Comparing Datasets")

![Transect Comparison](screenshots/compare_line.png "Transect Comparison")

![Area Comparison](screenshots/compare_area.png "Area Comparison")

## Changing Map Settings <img src="screenshots/settings_button.png" width=35 height=35 />

![Settings Window](screenshots/settings_window.png "Settings Window")

1. Map

   Projection

   the global projection will be the view that most users will need, however for users that want to view the north or south poles those options exist in the drop down here.

   Basemap

2. Color Interpolation

3. Bathymetry



