Triangulate Remote Location XY
==============================
The tool finds the coordinates of a remote object using observation coordinates and azimuths.
The triangulation data should include azimuths to an observed object from 3 points of observation and the coordinates of the observation points (in WGS84 decimal degrees).
The tool creates an estimate of error for the coordiante and displays it as a buffer of location around the estimated coordinate.

![triangulation](https://github.com/DmitriiSarychev/RemoteLocationXY-QGIS/assets/6863405/1a58e779-e8a2-40e6-b9a4-644b761facf2)

The input and output data are stored in a Comma Separate Value text file (.csv).
The name and folder of the output files could be choosen by user or left blank to use the default (subfolder "RemoteLocationXY" in the current QGIS project folder).
Basic information about the output is also displayed in the process log during the run.

Plugin in action
----------------
Click run button in the up right corner to see the process:
![rem_loc_xy](https://github.com/DmitriiSarychev/RemoteLocationXY-QGIS/assets/6863405/c347096d-5da0-459e-ad67-47e8888765d9)

How to install
------------
To use, download the zip-file "RemoteLocationXY.0.1.zip" and install it to QGIS 3.x via "Plugins -> Manage and install Plugins...-> Install from ZIP" or install via the tool repository as shown below.
1. From QGIS main menu go to "Plugins -> Manage and install Plugins...-> Settings"

![image](https://github.com/DmitriiSarychev/RemoteLocationXY-QGIS/assets/6863405/4ad14d74-9328-47e5-bf72-b8d2ee6def6d)
![image](https://github.com/DmitriiSarychev/RemoteLocationXY-QGIS/assets/6863405/61d6bd84-f618-485e-9a4b-9e1aba974286)

2. Click "Add..." button and input any name (e.g. "RemoteLocationXY") and the URL: https://github.com/DmitriiSarychev/RemoteLocationXY-QGIS/raw/main/plugin.xml

![image](https://github.com/DmitriiSarychev/RemoteLocationXY-QGIS/assets/6863405/4d6c6e57-d8d4-4a8a-8a42-fadc557a366b)

3. Press "Ok" and move to the "All" section of the Plugins manager, then start typing the tool name "triangulate..." in the search window

![image](https://github.com/DmitriiSarychev/RemoteLocationXY-QGIS/assets/6863405/93a67349-746d-40a8-96fc-ef3c767b875e)

4. Click on the name of the plugin as it comes up in the search list, then press the "Install" button in the buttom right corner.
The plugin installed. You can find it in the Processing Toolbox

![image](https://github.com/DmitriiSarychev/RemoteLocationXY-QGIS/assets/6863405/36fb4a61-724e-4f8c-a3d9-969007b74b02)

History
-------
The QGIS Remote Location XY plugin is based on the original tool, which was developed by Dorn Moore, Spatial Analyst and Dmitrii Sarichev, GIS Intern at the International Crane Foundation in 2014 and updated in 2020 to work with the latest version of ArcPy.
To use that ArcGIS based tool an ArcGIS license needed. So we reproduce all the functionality of the original tool using fully open source QGIS environment with PyQGIS by the 10th anniversary of the Remote Location XY.

References
----------
* Original git-project:
https://github.com/InternationalCraneFoundation/RemoteLocationXY

* The original tool page on the ArcGIS.com:
https://www.arcgis.com/home/item.html?id=ced07bf9669e44c38b2529175f14674f

* Short overview of the tool on YouTube:
https://www.youtube.com/watch?v=H510cmyLRtw&ab_channel=DmitriiSarychev
