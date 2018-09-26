
![very good|512x397](//renesasatces.com/wp-content/uploads/2017/12/Ushr-logo-300x87.jpg)

# Line2GPS 
A QGIS plugin to generate GPS samples along the Line or a specified  Route 
This plugin is only compatible with Qgis 2 (Python 2)
### Installation the plugin in Qgis 

  - Download the 7zip archive from `adm_exp`  downloads section https://bitbucket.org/ushrauto/adm_exp/downloads/Line2GPS.7z
  - Extract the archive to the QGis plugins directory (Windows - `C:\Users\username\.qgis2\python\plugins\` ) 
  - make sure it's extracted to it's own directory withn the `\python\plugins directory` 
  - Open QGis, Navigate to `Plugins` in the top menu bar and then  `Manage and install plugins...`
  - In the plugins window go to `Settings` tab on the left pane and chceck `Show also Expermimental plugins`
  - Go to the `Installed` tab on the left panel, you should now see `USHR-Line2GPS` listed in the available plugins 
  - Install the plugin , now you should see our great Company logo in the top plugins icons . Dont click that yet !  
  - You would need to create a new shapefile layer with type Line to start the plugin 
  

- By using the 3rd party plugin `Online Routing Maper` to automatically create a route between two points using Google Maps API/Tomtom/Here API .
then use our plugin to create GPS Points along that route ( Note - the generated route will not be lane level accurate or even could be out of rotue at tight corners )


### Plugin Parameters
  - `Distance between points` - Spacing between each GPS coordinate (Meters)
  - `Timedelta in GPS samples` - Specify frequency of GPS samples (Milliseconds)
  - `Altitude` - Manual height to report back in the GPS data (Meters)
  - `Output CSV file` - Directory to save the output Csv file 
 

 

### TODO's  
  - Implement auto route generation based on ADM Data Store with connecting Road Untis and Lanes table in sqlite file ( similar thirdparty `online Routing Maper` but to be specific with lane level )


