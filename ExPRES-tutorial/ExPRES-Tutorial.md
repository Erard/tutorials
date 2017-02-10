#ExPRES tutorial	
##Modeling, Analysis and Simulations of the Emissions in the Radio range. MASER Tool Suite User Guide

[Authors](#Authors)  
[Change Log](#Log)  
[Introduction](#1)  
[ExPRES](#2)  
&nbsp;&nbsp;&nbsp;[Connecting to ExPRES](#2.1)  
&nbsp;&nbsp;&nbsp;[ExPRES UI](#2.2)  
[SILFE](#3)  
&nbsp;&nbsp;&nbsp;[Connecting to SILFE](#3.1)  
&nbsp;&nbsp;&nbsp;[Datatree window](#3.2)  
&nbsp;&nbsp;&nbsp;[Plot Window](#3.3)  
[References](#References)

<h2 id="Authors">Authors</h2>

S. L. G. Hess  
sebastien.hess@onera.fr  

<h2 id="Log">Change Log</h2>

|Version|Name|Note|
|---|---|---|
|1|[Keyuan Yin](https://github.com/megadiesel705)|First converted from [this site](http://maser.obspm.fr/serpe/MASER_Guide_v0.2.pdf)|  


<h2 id="1">1.Introduction</h2>
Up do day, the MASER tool suite is composed of two online tools :  



<h3 id="2.1">Connecting to ExPRES</h3>
The ExPRES online tool address is (as of Sept. 2014) : http://typhon.obspm.fr/maser/serpe  

<img src="https://raw.githubusercontent.com/megadiesel705/tutorials/master/ExPRES-tutorial/img/1_F1.png" width="500" alt="1">  

*Figure 1: Font page of the ExPRES website*  




<h3 id="2.2">ExPRES UI</h3>

**Main page layout**  

<img src="https://raw.githubusercontent.com/megadiesel705/tutorials/master/ExPRES-tutorial/img/2_.png" width="500" alt="2_Layout">  

The ExPRES main page is composed of two parts the command panel (left) and the simulation setup panel (right).  



The results can be accessed by clicking on the expand button ￼ Results. Then the data can be viewed by clicking on their name. The XML outputs, which follows the IVOA VOTable standard can be shared with third-party VO applications though the SAMP protocol by clicking on the ￼ icon. This can be used to display the results in SILFE.  

**Simulation Setup panel**  

*General parameters*  

The time settings are limited to the times at which the simulation starts and ends (in minutes, like all times and durations in ExPRES) and the number of time steps.  


Frequency parameters are of three types that can be selected in a list (click on ￼ ). The linear and logarithmic scales are defined by minimum and maximum frequencies and the number of frequencies to simulate. Predefined frequencies also exist that corresponds to known instruments they can be selected by .  

*Observer*  

There are three types of observers : fixed ones whose position in the simulation reference frame does not vary ; orbiters which moves in the simulation reference frame, orbiting around a celestial body ; predefined observers which represent known mission around celestial bodies. To select the

<img src="https://raw.githubusercontent.com/megadiesel705/tutorials/master/ExPRES-tutorial/img/observer_1.png" width="500" alt="observer_1">  


<img src="https://raw.githubusercontent.com/megadiesel705/tutorials/master/ExPRES-tutorial/img/observer_2.png" width="500" alt="observer_2">


*Celestial bodies*  

Bodies can be created using the icon in the ￼ celestial bodies section (expend by clicking on ).  

<img src="https://raw.githubusercontent.com/megadiesel705/tutorials/master/ExPRES-tutorial/img/Celestial_body.png" width="200" alt="celestial bodies">  

*Density profiles*  


*Satellites*  

<img src="https://raw.githubusercontent.com/megadiesel705/tutorials/master/ExPRES-tutorial/img/satelites.png" width="200" alt="satellites">


**Sources**  


*Attached to a satellite*  

<img src="https://raw.githubusercontent.com/megadiesel705/tutorials/master/ExPRES-tutorial/img/attach_satelites.png" width="500" alt="attach_satelites">  

For source attached to a satellite, the satellite must be selected in the Satellite list (click on ￼ ).  

*Fixed in L-Shell*  

<img src="https://raw.githubusercontent.com/megadiesel705/tutorials/master/ExPRES-tutorial/img/L-shell.png" width="500" alt="L-shell">

For sources fixed in L-Shell, the field line motion is in corotation by default, but a subcorotation rate can be set in the “Subcorotation” field (0 = rigid corotation, 1 = no rotation at all).  

*Fixed in latitude*  

<img src="https://raw.githubusercontent.com/megadiesel705/tutorials/master/ExPRES-tutorial/img/latitude-fix.png" width="500" alt="latitude-fix">

For sources fixed in magnetic latitude, the field line motion is in corotation by default, but a subcorotation rate can be set in the “Subcorotation” field (0 = rigid corotation, 1 = no rotation at all).  

**Outputs**  

*Dynamic spectra*  

<img src="https://raw.githubusercontent.com/megadiesel705/tutorials/master/ExPRES-tutorial/img/dynamic-spectra.png" width="500" alt="dynamic-spectra">  

ExPRES standard outputs are dynamic spectra (intensity in the time-frequency domain). But ExPRES can also display the intensity as a function of observer or source longitude, source latitude, or local time or observer distance. This can be managed by selecting the corresponding checkboxes in the type section. The longitude/latitude/local time/distance ranges to be display must be specified in the corresponding fields.  



<img src="https://raw.githubusercontent.com/megadiesel705/tutorials/master/ExPRES-tutorial/img/dynamic-spectra_2.png" width="500" alt="dynamic-spectra-2">  

 
 
*2D movies*  

<img src="https://raw.githubusercontent.com/megadiesel705/tutorials/master/ExPRES-tutorial/img/2d-movie.png" width="300" alt="2d-movie">  

ExPRES can also display the position of the observed sources in the “field of view” of the instrument. This is done by adding a “2D movie” in the simulation (click on ￼ 2D movie).  


<img src="https://raw.githubusercontent.com/megadiesel705/tutorials/master/ExPRES-tutorial/img/2d-movie-2.png" width="300" alt="2d-movie-2">  

*3D movies*  

Then, it is needed to specify the spatial domain to be displayed. It is also needed to specify the subcycling for the movie, that is the number of simulation time steps between to successive pictures.  

<img src="https://raw.githubusercontent.com/megadiesel705/tutorials/master/ExPRES-tutorial/img/3d-movie.png" width="300" alt="3d-movie">  


<h2 id="3">3.SILFE</h2>

<h3 id="3.1">Connecting to SILFE</h3>




<h3 id="3.2">Datatree window</h3>

**Components**  

The datatree window is composed of the ￼ icon which permits to start a new plot window (there is no limits on the number of plot windows simultaneously opened).


<img src="https://raw.githubusercontent.com/megadiesel705/tutorials/master/ExPRES-tutorial/img/Components.png" width="300" alt="components">  

**Fields**  

<img src="https://raw.githubusercontent.com/megadiesel705/tutorials/master/ExPRES-tutorial/img/fields.png" width="300" alt="fields">

Observational datasets are marked with the ￼ icon at the


**Physical content of a field**  

SILFE may auto-detect the physical content of each field (from the UCD is specified in the data file), in which case it is displayed in parenthesis after the field name:  

<img src="https://raw.githubusercontent.com/megadiesel705/tutorials/master/ExPRES-tutorial/img/table.png" width="400" alt="table">  

When SILFE recognizes several physical contents in the same dataset, in generates new fields from those. These derived fields are marked with the ￼ icon. The fields from which they are computed are indicated in the parenthesis.  


**Catalog**  

Catalogs of radio emissions are also available in SILFE. Catalogs can be accessed by performing a right click on the dataset name. Then the catalog is accessed by clicking on the ￼ icon.  

<h3 id="3.3">Plot Window</h3>  

To open a plot window, click on the icon ￼ in the datatree window as shown of the figure on the right.  

<img src="https://raw.githubusercontent.com/megadiesel705/tutorials/master/ExPRES-tutorial/img/plotwindow.png" width="200" alt="plotwindow">  

**Plotting a field**  

<img src="https://raw.githubusercontent.com/megadiesel705/tutorials/master/ExPRES-tutorial/img/plot_field.png" width="200" alt="plot_field">

To plot a field in the plot window, select the corresponding dataset in the datatree and drag it (by keeping the left mouse button pressed) over the “ Figure X” label. A horizontal bar should appear below the label. Then drop it (release the mouse button). The detail of the field will appear on the left side of the window.  

**Save and share**  





<img src="https://raw.githubusercontent.com/megadiesel705/tutorials/master/ExPRES-tutorial/img/another_panel_plot.png" width="500" alt="plot_another_panel">  

**Overplotting a second field**  



<h2 id="References">References</h2>

Please refer this tutorial to original version on [this site](http://maser.obspm.fr/serpe/MASER_Guide_v0.2.pdf)