# openFlowApp

This README is a general guide to the use of the Flow2PowerTool.mlapp GUI and its inputs/outputs.  The tool was created to calculate the estimated power generation 
of an underwater kite from model generated water flow data.



##########

OPERATION

##########

To operate the program:

	1)  Locate the data input selection buttons in the leftmost column of the GUI.

		a)  Click the button for loading statistical NetCDF (*.nc) data and select the folder that contains your *.nc files.

		b)  Click the button for loading the kite’s power surface (*.mat) file and select the appropriate power surface file with the browser.

	2)  Set the operating parameters of your kite.
		a)  The minimum operating depth is the shallowest depth that the kite will be allowed to fly.
		b)  The ground masking depth is the deepest water column depth that the kite will be able to anchor itself.

	3)  Choose a processing method (Process or Quick Process).  The “Quick Process” button will process the data much faster than the standard “Process” button.  The
	standard “Process” button takes ~30 times longer due to a finer grain power conversion interpolation operation.  The “Process” button produces expected power 
	estimates that are generally thousandths (~0.001 kW) of a kilowatt higher than the “Quick Process” method.  Because of the incredibly small differences in expected 
	power between the two methods, the “Quick Process” option is the better option for a quick look at a dataset.


	4)  Once a processing method has been selected, a loading bar will appear and update as the process operations are completed.



##########

Output

##########


Once the processing has completed, the plots and figures will update with information about the expected power over the test site area.

	1)  The center column’s top plot displays the monthly expected power generation at various site selection percentiles.  Below the plot is a table displaying 
	the values of expected power generation at the 25th, 50th, 75th, and 95th percentiles of site selection.

	2)  The right hand column of the GUI shows the depth profiles for flow speed and expected power for the water column with the highest yearly mean expected
	power within the test site.
	



%%%%
Data Format
%%%%

Data must be in chronological order.


