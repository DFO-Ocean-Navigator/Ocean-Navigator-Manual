# Ocean Navigator User Manual (v9.6)

The Ocean Navigator is a data visualization tool that enables users to discover and view ocean model output and observations quickly and easily. All model nowcast and forecast information are based on hydrodynamic models and should be considered as computer-generated guidance. These are an estimate of the oceanographic environment (i.e. potential temperature, salinity, and currents) and not directly measured in-situ observation of ocean conditions. The reanalysis products available though the Ocean Navigator are developed to be as close as possible to collected ocean observations and in agreement with model physics, giving a backward looking description of the ocean environment.

For specific technical specifications of each forecast or reanalysis product please consult the source at the links provided.

# Ocean Navigator Overview

![Ocean Navigator Overview](images/overview.png "Ocean Navigator Overview")

### 1. Global Map

The _global map_ is the most prominent way to visualize oceanographic forecast models in the Ocean Navigator. The default view is centered on the North-West Atlantic but users can pan over map clicking and dragging at any point. Users can also zoom in or out using their mouse wheel, laptop touchpad, or by using the zoom buttons in the [Additional Options](#5-additional-options) area.

The map is highly customizable and users are given the ability to change the map projection, basemap layers, bathymetry, and more. See [Changing Map Settings](#changing-map-settings-) for more details.

### 2. Dataset Selection Panel

![Dataset Selection Panel](images/dataset_selector.png "Dataset Selection Panel")

The dataset selection panel allows users to view datasets from the Ocean Navigator's data catalog on the global map. There are several menus that users can select data from. Once the user has selected a data product and the relevant parameters they must click the _Go_ button to display the data on the global map. The dataset selection menus are described in detail below.

1. Dataset Selector

   ![Dataset Dropdown Menu](images/dataset_dropdown.png "Dataset Dropdown Menu")

   The dataset dropdown allows users to select data from one of the many forecast models available in the Ocean Navigator. Within the dataset dropdown menu data is first grouped by forecast then other important characterisctics such as dimensionality, time range, and climatologies.

2. Variable Selector

   This dropdown menu allows users to choose a variable from the currently selected dataset.

3. Quiver Selector

   Users can overlay vector variables as quiver arrows over the global map view by selecting a variable from the quiver dropdown menu. The quiver overlay adjusts to the map zoom level and users can also use the _Quiver Density_ slider to fine tune the display.

   ![Quiver Arrows](images/quiver_arrows.png "Quiver Arrows")

4. Depth Selector

   This dropdown menu allows the user to change the depth level of the currently selected dataset for three dimensional datasets. The highest level is selected by default and the selector will not appear for two dimensional datasets.

5. Compare Datasets Switch

   This switch allows users to display two datasets simultaneously and make comparison line and area plots between the two. See [Comparing Datasets](#Comparing-Datasets) for more details on how to use this feature.

6. Timestamp Slider
   ![Time Slider](images/time_slider.png "Time Slider")

   Users can select the model forecast time on the global map using the _timestamp slider_. The currently selected time is indicated by the slider thumb <img src="images/slider_thumb.png" width=20 height=20 />.

   To select a new timestamp users can click on any tick along the timestamp slider or select an adjacent timestamp using the previous and next buttons located on each end of the slider <img src="images/chevron.png" height=20 />.

   Due to size constraints the timestamp slider only displays labels for major ticks at 00:00 and 12:00 for hourly datasets but a tooltip will appear over the minor ticks to indicate their values. For datasets with time ranges beyond the currently displayed timestamps the <img src="images/double_chevron.png" height=20 /> buttons can be used to change which group of timestamps are displayed.

7. Hide Data Lay Button

   This button allows users to toggle display of the data layer and view underlying bathymetry. 

8. Go Button

   The _Go Button_ is used to enact the changes that the user has made through the menus above.

### 3. Colormap Scale Viewer

![Colormap Scale Viewer](images/scale_viewer.png "Colormap Scale Viewer")

The _Colormap Scale Viewer_ displays the value range the currently displayed variable. Clicking on the data scale viewer will reveal the _Colormap Range_ selector. Here users can adjust the maximum and minimum values of the current colormap by entering new values, or clicking the _Auto_ button which will scale the colormap to the data range within the area currently visible on the map. Clicking _Default_ will restore the original colormap range.

### 4. Ocean Navigator Map Tools

#### Draw Map Features <img src="images/draw_button.png" width=35 height=35 />

Clicking this button enters drawing mode and the Navigator's drawing options are displayed. The drawing options provide buttons to change the drawn feature type (point, line, or area), undo a point, clear the map, and plot the features added by the user. Once points have been added to the map their locations can also be modified using the [Edit Map Features window](#edit-map-features). For more details on drawing coordinates and plotting see [Adding Map Features with the _Draw Map Features_ Tool](#adding-map-features-with-the-draw-map-features-tool).

#### Edit Map Features <img src="images/edit_button.png" width=35 height=35 />

Selecting this option displays the _Edit Map Features window_. This feature allows users to enter the exact location of points of interest and plot data at those locations. Users also have the option of importing coordinates from a CSV file. Like the _Draw Map Features_ tool, users can select from a the standard feature types and plot the selected data. Any points present on the map, whether they have been previous entered though this window, imported from a CSV, or drawn on the map, can be modified in this window. See [Adding and Modifying Map Features with the _Enter Point Coordinates_ Tool](#adding-and-modifying-map-features-with-the-edit-map-features-tool) section for more information.

#### Preset Features <img src="images/preset_button.png" width=35 height=35 />

The Ocean Navigator also provides users with a number of preset points, lines, and areas that may be of interest to users. Clicking on this button will present the user with a menu where they can select one of these features and add it to the map. Once added, features can be plotted by clicking on them. Note that selecting any of these options will remove any other features from the map.

#### Observations <img src="images/obs_button.png" width=35 height=35 />

The _Observations_ button allows users to access the Ocean Navigator's observations database. When clicked the Observation options which gives the user a number of options for selecting observations or displaying Class4 data. For a more detailed description of these options see [Viewing Observation and Class4 Data](#viewing-observation-and-class4-data).

#### Plot <img src="images/plot_button.png" width=35 height=35 />

The _Plot_ button behavior is dependent on the data displayed on the map. For user selected point, lines, or areas clicking this button will open the appropriate [plot window](#ocean-navigator-plot-windows). In the event that multiple points were selected the resulting plot will contain all of them. For preset features, observations, and Class4 points clicking this button will open a plot window for the most recently selected feature.

#### Reset Map <img src="images/reset_button.png" width=35 height=35 />

The _Reset Map_ button removes all features from the map.

#### Settings <img src="images/settings_button.png" width=35 height=35 />

This button will open the [settings window](#changing-map-settings) where users can modify the global map.

#### Info/Help <img src="images/info-help_button.png" width=35 height=35 />

Clicking this button opens the _Info/Help_ window where users can find dataset metadata, variable definitions, and help documents, including this one.

### 5. Additional Options

![Additional Options](images/additional_options.png "Additional Options")

1. Add Map Annotation Button

   Allows users to add labels to the map. See [Adding Map Annotations](#adding-map-annotations) for more detail.

2. Get link Button

   This button opens the _Share Link_ window. Here, users can generate a link to the current state of the Ocean Navigator and share it with others. When accessing the application through this link the current dataset options will be restored.

3. Language Selector

   Allows users to toggle between English and French.

4. Cursor Coordinates

   Displays the current latitude/longitude coordinates of the mouse cursor.

5. Zoom Buttons

   These buttons can be used to change the zoom level of the global map.

# Ocean Navigator Plot Windows

Users can produce a number of plot types from points of interest within the Ocean Navigator. Each plot includes basic statistics for the data presented.

## Point

![Point Window](images/point_window.png "Point Window")

The _Point_ window contains a number of plot types appropriate for extracting data from individual point coordinates.

1. Plot Tabs

   Here users can select from a number of point plotters:

   - **Profile Plot:** This is a plot along the water column at the chosen location(s). This plot is only available for variables with a depth dimension. Multiple variables can be selected from the _Dataset Selector_ by holding the shift key and clicking on the desired variables. See _2. Dataset Selector_ for more information.
   - **CTD Profile:** Similar to the _Profile Plot_ but only displays temperature and salinity data.
   - **T/S Diagram:** A temperature and salinity diagram for the selected location. Temperature is given on the vertical axis and salinity on the horizontal. The figure's depth values are amended to the resulting line.
   - **Sound Speed Profile:** A profile plot for the Sound Speed variable. The horizontal axis ranges from 1410 to 1560 m/s.
   - **Observation:** See [Observation](#observation).
   - **Virtual Mooring:** A timeseries plot of at the chosen location. Users can specify start and end times of the plot but due to resource constraints only 50 timestamps can be displayed at once.

2. Global Settings

   Similar to the global map's Dataset Selector. Here users can change the dataset, variable, and other parameters. Depending on the current plot tab selected these options may change. The Profile plotter allows users to select multiple variables to be displayed by holding shift and clicking on the variables of interest. This plot, and the virtual mooring plot also include a range selector that allows the user to modify the dependent variable axis range in the plot. When the Virtual Mooring tab is selected the dataset selector will include a time selector for the start and end times of the plot. The user can also check the _Show Location_ box to display a map of the points within the plot. Here they can also change the location of the selected point. The _Plot Options_ menu allows users to adjust the plot's size and provide an alternate title.

3. Save Options

   See [Saving Plot Images and Data](#saving-plot-images-and-data).

## Line

![Line Window](images/line_window.png "Line Window")

The _Line_ window plots data along a route specified by two or more point coordinates.

1. Plot Tabs

   - **Transect:** A transect plot displays the values along the selected line and water column. The data values are given by the colormap on the right. This plot is only available for variables with depth dimensions.

   - **Hovmöller:** A Hovmöller diagram displays the values along the selected line over a period of time. Again, data values are given by the provided colormap.

2. Global Settings

   This panel provides the following options for the selected plot.

   - **Compare Datasets:** Checking this option allows users to compare two variables from any of the Ocean Navigator datasets along the selected line.
   - **Show Map Location:** Check this option to include a map of the selected line in the plot (checked by default).
   - **Plot Options:** Allows users to adjust the plot's size and provide an alternate title.

   If a _Transect_ plot is selected:

   - **Surface Variable:** Users can plot the surface values along the transect for any variable listed in the dropdown menu.
   - **Linear Threshold:** This threshold separates the plot into two sections. The values above the threshold value are plotted on a linear scale while those below are plotted on a logarithmic scale.
   - **Depth Limit:** This option limits the depth of the transect plot.

3. Save Options

   See [Saving Plot Data and Images](#saving-plot-images-and-data).

4. Main Map (Dataset Selector)

   Similar to the global map's Dataset Selector. Here users can change the dataset, variable and other parameters. if _Compare Datasets_ is checked then a second dataset selector will become available. This dataset selector also allows users to change the colormap of the plotted data.

## Area

![Area Window](images/area_window.png "Area Window")

The _Area_ window plots data within a polygon specified by three or more point coordinates.

1. Area Settings

   This panel provides the following options for the selected plot.

   - **Compare Datasets:** Checking this option allows users to compare two variables from any of the available datasets along the selected line.
   - **Show Bathymetry Contours:** This option adds bathymetry contours to the area plot (checked by default)
   - **Show Selected Areas:** Checkbox indicated whether to include the selected area in the plot (checked by default).
   - **Arrows Menu:** Selecting a variable from this menu adds its quiver arrows to the area plot.
   - **Additional Contours:** Selecting a variable from this menu adds its isolines to the plot.
   - **Plot Options:** Allows users to adjust the plot's size and provide an alternate title.

2. Subset Panel

   The subset panel allows users to extract data from the plotted area and download in a number of NetCDF file formats. NetCDF files contain self-describing, array-oriented scientific data.

   - **Variables:** Users can select one or more variables to add to the NetCDF subset product from this menu. To select multiple variables hold the shift key while making a selection.
   - **Select Time Range:** Checking this box will allow users to create a subset over a time range.
   - **Time Selector:** Specify the timestamp for the subset data. If a time range is selected two selectors will allow users to pick the start and end times.
   - **Output Format Dropdown:** Users can chose from a number of NetCDF formats for the output.
   - **Compress as \*.zip:** Checking this box will compress the output file in a .zip archive.
   - **Save:** Once all of the above have been selected click this button so save the subset product.
   - **API Scripts:** Users can download API scripts to retrieve the selected subset data in _R_ or _Python_.

3. Save Options

   See [Saving Plot Images and Data](#saving-plot-images-and-data).

4. Dataset Selector

   Similar to the global map's Dataset Selector. Here users can change the dataset, variable and other parameters. if _Compare Datasets_ is checked then a second dataset selector will become available. This dataset selector also allows users to change the colormap of the plotted data.

## Observation

![Observation Window](images/obs_plot_window.png "Observation Window")

The _Observation_ window allows users to compare a selected observation to model data. The observation window will contain two figures with the observtion data on the left and model data on the right.

1. Dataset Selector

   A limited dataset selector where users can change the dataset and its timestamp, and the location of the point compared to the observation. Since the selected dataset may not contain data from the same time as the observation the most recent timestamp is selected by default. This dataset selector also includes an _Observation Variables_ list where users can choose which observed metric to compare to the model.

2. Save Options

   See [Saving Plot Images and Data](#saving-plot-images-and-data).

## Class4

![Class4 Window](images/class4_window.png "Class4 Window")

Class4 metrics are one of a number of validation tools used to validate GIOPS or RIOPS model forecasts by comparing temperature and salinity predictions to observations of the same quantities.

1. Class4 Settings

   - **Show Location:** Check this option to include a map of the selected line in the plot.
   - **Show Climatology:** Check this option to include climatology data in the figures.
   - **Additional Models:** Users can also add other models to the figures to comparison. To add multiple hold the shift key while selecting models.
   - **Show Error:** Check this option to view the error of the models compared to the observation.
   - **Plot Options:** Allows users to adjust the plot's size and provide an alternate title.

2. Save Options

   See [Saving Plot Images and Data](#saving-plot-images-and-data).

## Saving Plot Images and Data

The are three sets of options available to users for extracting the plotted data:

**Save Image**

Users can save the plot in one of many common image formats including _png, jpg, svg_, and others. The _CSV/ODV_ options allow the user to download the raw data in either format. Lastly, users can download just the statistics using the _Statistics (csv)_ option.

**Get Link**

Here users can generate links to the plotted data. The _Web_ option will produce a link that will open the Ocean Navigator in its current state with the plot window opened and plot displayed. The _Image_ option creates a direct link to the image only.

**API Script**

Users can generate API scripts in either _R_ or _Python_ that will fetch the plot. The _PLOT_ option will retrieve the image in _png_ format while the _csv_ option will produce a _csv_ file containing the plot data. These options can be further developed to include other Ocean Navigator features. See the [API Documentation](https://navigator.oceansdata.ca/docs) for further information on how to interact with the API.

# Using the Ocean Navigator

## Adding Map Features with the _Draw Map Features_ Tool

To select points of interest on the global map first clicking on the _Draw Map Features_ button <img src="images/draw_button.png" width=35 height=35 /> to open the drawing options:

![Drawing Options](images/drawing_tools.png "Drawing Options")

These options include:

- _Point_, _Line_, and _Area_ toggle:

  These buttons are used to toggle between the drawn feature type. To complete a line or area double click at the ending location. Area features can also be completed by clicking on the starting point.

  ![Points, Line, and Area](images/point_line_area.png "Points, Line, and Area")

- _Clear_ button:

  This button will remove all features from the map.

- _Undo_ button:

  This button removes the last-drawn feature.

- _Close_ button:

  Closes the plot options.

![Drawing Map Features](animations/map_features/add_feature_click.gif "Drawing Map Features")

Once features have been drawn user can select a feature to plot by clicking on it. Only one line or area feature can be selected at a time but multiple points can be selected at once. To do so hold the _shift_ key while clicking on the desired point features. Selected features can be deselected by holding shift and clicking on them.

Selected features can be plotted by double clicking on them or pressing the plot button on the right side of the screen <img src="images/plot_button.png" width=35 height=35 />. All selected point features will be plotted together.

![Plotting Map Features](animations/map_features/plot_features.gif "Plotting Map Features")

Users can add as many points as they wish by clicking on the map. To modify features users can open the _Edit Map Features_ window <img src="images/edit_button.png" width=35 height=35 /> to modify feature coordinates, change a feature's geometry type, or remove a feature from the map. 

## Adding and Modifying Map Features with the _Edit Map Features_ Tool

Users can precisely add new features and edit existing ones using the _Edit Map Features_ tool. <img src="images/edit_button.png" width=35 height=35 />

![Edit Map Features Window](images/edit_map_features.png "Edit Map Features Window")

The left side of the window contains a _feature card_ for each one currently drawn on the map. Feature cards contain functionality for modiying coordinates, geometry, and labels. Clicking _Add New Feature_ will add an empty feature card to the feature list. From there users can add points to the feature using the _Add Vertices (+)_ button.

![Add Feature with Edit Map Features Window](animations/map_features/add_feature_table.gif "Add Feature with Edit Map Features Window")

![Adding Feature Vertices with Edit Map Features Window](animations/map_features/add_vertices.gif "Adding Feature Vertices with Edit Map Features Window")

A feature's geometry type can be changed using the drop down menu at the top of the feature card. 

![Change Feature Type with Edit Map Features Window](animations/map_features/change_feature_type.gif "Change Feature Type with Edit Map Features Window")

Users can also add labels to features by adding text to the text box at the top of the feature card.

![Add Feature Label with Edit Map Features Window](animations/map_features/label_features.gif "Add Feature Label with Edit Map Features Window")

Users can select and de select features by clicking on the check box in the top left corner of each feature card. If one or more features is selected the _Plot Selected Features_ button will be enabled.

Users can modify feature coordinates by editing the values in the feature cards. Vertices can be remoted entirely by clicking the _X_ to the right of the coordinate boxes.

Multiple selected point features can be combined into a single feature using the _Combine Selected Point Features_ button. The combined points will create a line feature by default but can be changed to an area using the geometry type dropdown. Likewise, selected line and area features can be split into individual point features by clicking on the _Split Line/Area Feature Into Points_ button.

![Combine Point Features with Edit Map Features Window](animations/map_features/combine_points.gif "Combine Point Features with Edit Map Features Window")

![Split Line/Area Features with Edit Map Features Window](animations/map_features/split_poly.gif "Split Line/Area Features with Edit Map Features Window")

Users can also import data from _csv_files by clicking on the \_Upload CSV_ button. The uploaded type can be selected using the adjacent dropdown menu. The file must begin with a header containing "latitude" and "longitude" to indicate which columns hold these values.

Users can click on values in the table to make further changes, or remove them completely by clicking the _x_ icon on the right of their respective rows.

![Add Feature with Edit Map Features Window](animations/map_features/add_feature_table.gif "Add Feature with Edit Map Features Window")

## Creating Plots via the _Preset Features_ Menu

The Ocean Navigator also has a number of preset features that may be of interest to users. To view the list of the preset features click on the _Preset Features_ button <img src="images/preset_button.png" width=35 height=35 />

![Preset Features Window](images/preset_features_window.png "Preset Features Window")

Features are categorized into lists of Point, Line, or Area features. Click on any item from the list to add it to the global map. Note that any other features will be removed.

![NAFO Divisions](images/NAFO_areas.png "NAFO Divisions")

Once features are added to the map users can plot their point/line/area data by clicking on them.

## Removing Map Features

Users can remove features from the map using one of the following methods:

   1. Using the Undo button in the _Draw Map Features_ menu to remove the last-added feature.
   2. Deleting specifc features the Edit Map Features window.
   3. Clicking Reset Map button to remove all features from the map.

![Removing Map Features](animations/map_features/remove_features.gif "Removing Map Features")

## Viewing Observation and Class4 Data

The Ocean Navigator has a variety of observation products available to its users. To
display observation features on the map first click the _Observations_ button <img src="images/obs_button.png" width=35 height=35 />. This will open the _Observation Options_ menu:

![Observation Options](images/obs_tools.png "Observation Options")

These options are as follows:

- _All:_

  Select this option to view observations without any geographic constraints. This immediately opens the _Select Observations_ window.

- _Select Area:_

  This option allows users to view observations within a chosen area. When clicked the user is prompted to draw an area polygon before the _Select Observations_ window is opened.

- _Select Point:_

  The _Select Point_ option allows users to select observation within a radius of a given coordinate. When clicked users will need to click on the desired location on the map to open the _Select Observations_ window.

- _Class4:_

  This option opens the _Class4 Selector_ used to view Class4 data. See [Displaying Class4 Data](#displaying-class4-data).

- _Close:_

  Click this button to close the _Observation Options_ menu.

Once a selection has been made the _Select Observations_ window will open. This window gives users a number of ways to query observation data and view the resulting products.

![Observation Window](images/obs_window.png "Select Observation Window")

1. Observation Type

   Here users can choose to view the observation product as individual points or tracks on the map.

2. Date & Variable Filters

   Here users can specify a date range for the resulting observation data and the observed variable.

3. Platform Filters

   This menu allows users to narrow their observation query to a specific plat form type. From there they can restrict their search to platforms matching a specific Metadata Key such as instrument identification numbers, name of the principal investigator, ship name, and more. These criteria are not applied to the search unless the switch is active.

4. Depth Filter

   This slider can be used to restrict observations to a particular depth range in the water column. Like the _Platform Filters_, this range is not applied unless the switch is active.

5. Apply

   Click _Apply_ to query the observations once all of the selections have been made.

Once the user has completed the steps above the global map will be populated with observation points that meet their selection criteria.

![Observations displayed on map](images/observations.png "Observations displayed on map")

### Displaying Class4 Data

Selecting the Class4 button from the _Observation Options_ opens the _Class4 Selector_. Class4 metrics are one of a number of validation tools used to validate GIOPS or RIOPS model forecasts by comparing temperature and salinity predictions to observations of the same quantities.

Class4 metrics are available in two categories; _Ocean Predict_, and _RIOPS Assimilated Observations_. _Ocean Predict_ products are Class4 validation products that compare data from the GIOPS forecast model against observations. This product also includes forecasts from other models which can be added to the comparison plots. The _RIOPS Assimilated Observations_ products are similar but only include data from the RIOPS forecast model.

The _Class4 Selector_ includes a dropdown menu to where users can toggle between to two Class4 product types and a calendar that shows the dates with available data for the selected product.

![Class4 Selector](images/class4_selector.png "Class4 Selector")

To add Class4 data to the map select the Class4 product type then a date of interest. The Ocean Navigator will then draw the Class4 points on the map. These points are colored according the products RMS error i.e. how well the model fits the observed data. Green points indicate high agreement between the forecasted data and observation while red points indicated poor agreement.

![Class4 points displayed on map](images/class4_points.png "Class4 points displayed on map")

## Comparing Datasets

Checking the compare datasets toggle switch ![Compare Datasets Toggle](images/compare_toggle.png "Compare Datasets Toggle")
will open the comparison view. The view includes two maps and corresponding Dataset Selector panels. Users can select from any two available datasets and make comparisons between them. Any map interactions, such as panning or zooming, is applied to both maps. Feature selection will also apply to both maps and comparison plots will be made where possible. Examples of the comparison view and resulting transect and area plots are given below.

### Comparing datasets on the Global Map
![Comparing Datasets](images/compare_map.png "Comparing Datasets")

### Comparing Transect plots
![Transect Comparison](images/compare_line.png "Transect Comparison")

### Comparing Area plots
![Area Comparison](images/compare_area.png "Area Comparison")

## Changing Map Settings <img src="images/settings_button.png" width=35 height=35 />

![Settings Window](images/settings_window.png "Settings Window")

Users can change many of the Global Map parameters to suit there needs. The available options are described below:

1. Map

   - _Projection:_

     Users can toggle between the Global (default), Arctic, or Antarctic projections.

   - _Basemap:_

     Users can change the topography of the land and underlying bathymetry with this dropdown menu.

2. Color Interpolation

   Because the model forecast data is discrete and can be relatively sparse interpolation is used to smooth and fill in areas on the maps data tiles.

   - _Method:_

     Users can change the interpolation method applied to the data tiles. _Gaussian Weighting_ is used by default but other methods, such as Bilinear and Nearest Neighbour interpolation, can be used instead.

   - _Sampling Radius (km):_

     The distance from each point used in the interpolation calculation.

   - _Nearest Neighbours:_

     The number of neighbours to use in the interpolation calculation.

   - _Apply:_

     Click this button to apply interpolation changes to the map.

3. Bathymetry

   - _Show Bathymetry Contours:_

     This checkbox allows users to toggle the bathymetry contours drawn on the global map.

   - _Bathymetry Opacity:_

     Here users can adjust the opacity of the bathymetry contours.

   - _Bathymetry Layer:_

     This menu will allow users to select between bathymetry sources. At the moment only _ETOP01_ is available.

   - _Topography Shaded Relief:_

     Check this box to add shaded relief to the basemap layer.

   - _Apply:_

     Click this button to apply bathymetry changes to the map.

## Adding Map Annotations

Users can now add labels to the map to indicate areas of interest or groups of features. The Add Annotation window allows users to add a new label, undo the most recently added, or clear all labels from the map. Labels can be moved by clicking on a dragging them.

![Adding Map Annotations](animations/map_annotations.gif "Adding Map Annotations")

# Instructional Videos

Please note that the following resources were created with a previous version of the Navigator and may not accurately depict current usage.

## Create Point plot and Virtual Mooring

<iframe
  width="853"
  height="480"
  src="https://www.youtube.com/embed/gcmjtYSJs8c"
  frameBorder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
  allowFullScreen
  title="Ocean Navigator: Create point plot and virtual mooring"
  >
</iframe>

## Create Virtual Mooring for current and bearing data

<iframe
  width="853"
  height="480"
  src="https://www.youtube.com/embed/pzzFh8cOLog"
  frameBorder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
  allowFullScreen
  title="Ocean Navigator: Create Virtual Mooring for current and bearing data"
  >
</iframe>

## How to modify Point plot range and add multiple variables

<iframe
  width="853"
  height="480"
  src="https://www.youtube.com/embed/NbB9iOoagiA"
  frameBorder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
  allowFullScreen
  title="Ocean Navigator: How to modify point plot range and add multiple variables"
  >
</iframe>

## Create Transect and Hovmöller plot

<iframe
  width="853"
  height="480"
  src="https://www.youtube.com/embed/zYoSJq306XI"
  frameBorder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
  allowFullScreen
  title="Ocean Navigator: Create Transect and Hovmöller plot"
  >
</iframe>

## Create Area plot and save \*.csv

<iframe
  width="853"
  height="480"
  src="https://www.youtube.com/embed/pid28Nuh3CQ"
  frameBorder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
  allowFullScreen
  title="Ocean Navigator: Create Area plot and save *.csv"
  >
</iframe>

## Subset NetCDF file and save

<iframe
  width="853"
  height="480"
  src="https://www.youtube.com/embed/QIDEgiDuUqI"
  frameBorder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
  allowFullScreen
  title="Ocean Navigator: Subset NetCDF file and save"
  >
</iframe>

## Creating plots using Enter Point Coordinates and adding quivers

<iframe
  width="853"
  height="480"
  src="https://www.youtube.com/embed/PqJ99yOG7WI"
  frameBorder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
  allowFullScreen
  title="Ocean Navigator: Creating plots using Enter Point Coordinates and adding quivers"
  >
</iframe>

## Creating climatology plots for predefined areas

<iframe
  width="853"
  height="480"
  src="https://www.youtube.com/embed/MCCmcexArXA"
  frameBorder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
  allowFullScreen
  title="Ocean Navigator: Creating climatology plots for predefined areas"
  >
</iframe>

## Plotting in-situ ocean Observation

<iframe
  width="853"
  height="480"
  src="https://www.youtube.com/embed/9hAgSWPVP9Q"
  frameBorder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
  allowFullScreen
  title="Ocean Navigator: Plotting in-situ ocean Observation"
  >
</iframe>

## Plot Class4 data

<iframe
  width="853"
  height="480"
  src="https://www.youtube.com/embed/ABid30zxSfc"
  frameBorder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
  allowFullScreen
  title="Ocean Navigator: Plot CLASS4 data"
  >
</iframe>

## Compare datasets and save plot

<iframe
  width="853"
  height="480"
  src="https://www.youtube.com/embed/tu44-hjqY0o"
  frameBorder="0"
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
  allowFullScreen
  title="Ocean Navigator: Compare datasets and save plot"
  >
</iframe>
