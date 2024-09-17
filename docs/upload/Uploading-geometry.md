## Upload existing lines
Up to this point, only drawing segments in the tool has been discussed. If you have existing lines representing project locations you want to analyze using LINK, they can be  uploaded directly and do not need to be re-drawn manually.

To do this, you need a **GeoJSON**, which is similar to a shapefile, but optimized for the web. A shapefile, or any other spatial data, can be turned into into a GeoJSON. 

To pre-name segments, add a 'name' field to the GeoJSON. Otherwise, you will be able to name the collection of segments, but they will follow the format 'Study1,' 'Study2,' etc..., where study is the name that you provide. 
But if you add a 'name' field, LINK will use those segment names in your outputs, which is helpful when reviewing a CSV output from LINK or when joining data. 

Note that LINK strips special characters out. To ensure a smooth re-join, it is recommended to use a unique ID in the name field. One way to do so would be to duplicate an existing UID column and cast it to a string data type.

Make sure that the 'name' column is of the data type 'string' or 'text,' others will not work. 

!!! note

    The GeoJSON **must** be in the EPSG: 4326 projection (WGS 1984). 
    If files are in another format, ArcGIS or QGIS can be used to export the lines as GeoJson. 
    Alternatively, online tools are available to convert shapefiles to GeoJSON.

    [How to convert a shapefile to a GeoJSON in ArcGIS Pro](https://pro.arcgis.com/en/pro-app/3.1/tool-reference/conversion/features-to-json.htm)

    [How to convert a shapefile to a GeoJSON in QGIS](https://support.tygron.com/wiki/How_to_create_a_GeoJSON_in_QGIS)


Once a GeoJSON of lines in the correct projection is ready:

- Click the Upload existing line(s) button
- Select the GeoJSON file
- Once uploaded, the line or lines appear on the map. If multiple lines have been uploaded, decide whether to run them individually, or to run them as one (to see the total benefit of building all of them)
    - If you run individually, make sure the lines are uncombined by clicking the S button to select all, then the uncombine button.
    - If the lines are run them as one project, click the S button to select all segments, then the combine button to combine them into one feature. 
- Click Analyze, name the study, and click Submit. Results will appear in the My Studies panel.
- Click the My Studies button at the top to open the panel 
- Click the Clear button to remove the results from the map before making another study or uploading additional features. 
Results can be reloaded into the map through the My Studies panel, by clicking View Study.


!!! note

    The chosen segments will be run exactly as they are segmented. 
    In other words, each row in the GIS attribute table will be run separately, unless the segments are combined in LINK. 
    Alternatively segments can be dissolved in GIS and grouped as desired.
