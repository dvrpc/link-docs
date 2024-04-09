## Upload existing lines
Up to this point, we've only discussed drawing segments in the tool. If you have existing lines representing the location of the projects you want to analyze using the LINK tool, 
you can upload them directly to the tool and do not need to re-draw them manually. 

To do this, you need a **GeoJSON**, which is similar to a shapefile, but optimized for the web. You can turn a shapefile, or any other spatial data, into a GeoJSON. 

!!! note

    The GeoJSON **must** be in the EPSG: 4326 projection (WGS 1984). 
    If your projects are in another format, you can use ArcGIS or QGIS to export the lines as GeoJson. 
    Alternatively, online tools are available to convert from shapefiles to GeoJSON.

    [How to convert a shapefile to a GeoJSON in ArcGIS Pro](https://pro.arcgis.com/en/pro-app/3.1/tool-reference/conversion/features-to-json.htm)

    [How to convert a shapefile to a GeoJSON in QGIS](https://support.tygron.com/wiki/How_to_create_a_GeoJSON_in_QGIS)


Once you have a GeoJSON of lines in the correct projection:

- Click the Upload existing line(s) button
- Select your GeoJSON file
- Once uploaded, the line or lines appear on the map. If you uploaded multiple lines, you should now decide if you'd like to run them individually, or if you want to run them as one (to see the total benefit of building all of them)
    - If you choose to run them individually, make sure they are uncombined by clicking the 'S' button to select all, then the uncombine button.
    - If you choose to run them as one project, click the 'S' button to select all segments, then the combine button combine them into one feature. 
- Click Analyze , name your project, and click Submit. Results will appear in the My Studies panel.
- Click the My Studies button at the top to open the panel 
- Click the Clear button to remove the results from the map before making another study or uploading additional features. 
Results can be reloaded into the map through the My Studies panel, by clicking 'View Study'.


!!! note

    Your segments will be run exactly as they are segmented.
    In other words, each row in your attribute table in GIS will be run separately, 
    unless you combine your segments in LINK, or 'dissolve' them in GIS to group them as you want them to be analyzed.

