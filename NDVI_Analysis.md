The core idea behind this analysis is to analyze how is a 26-hectare sacred grove responding to the ecological pressures exerted by 16 industrial establishments within its 1-km surrounding landscape?
Research questions:1. What is the vegetation condition of Shivbari sacred Grove? 2. How has vegetation changed between 2017 to 2026? 3. How much industrial and built-up pressure surrounds the grove? 4. Does the grove retain relatively better vegetation condition than its industrial surroundings?

Step: Area of Interest (AOI) Selection and Satellite Imagery Visualisation
   - Tool used: Copernicus Browser
   - In this step, I used the Copernicus Browser to visually inspect recent satellite imagery of my study area and define the Area of Interest (AOI) for analysis.
Procedure:
   - Opened the Copernicus Browser and logged in to my account, then switched to the Visualise tab.
   - Selected the data collection: Sentinel-2, with the Sentinel-2 L2A product (atmospherically corrected, surface reflectance data) chosen instead of L1C.
   - Chose the acquisition date: 2017-03-01-2017-03-31, which has a low cloud cover of 9%, giving a clear view of the land surface.
   - Kept the default configuration for the true-colour visualisation of the layer.
   - Drew a rectangular AOI on the map using the polygon/rectangle drawing tool. The selected area is approximately 3.59 km².
   - Placed a location marker at the centre of the AOI, which sits on a dense green vegetation patch (Shivbari Sacred Grove), surrounded by agricultural fields, bare land, and built-up areas. The NH3 road label is visible near the bottom of the AOI, which helps with geographic reference.
<img width="1892" height="863" alt="Screenshot 2026-11-10 220004" src="https://github.com/user-attachments/assets/0182a26d-986c-4d6d-9341-9cf65a4e6e8f" />

**Creation of the Surrounding Zone Using Erase:**
To isolate the surrounding landscape from the sacred grove itself, the Erase geoprocessing tool was used.
Tool: Analysis → Tools → Erase
 -Input Features- SacredGroveBoundary_Buffer1000m
 -Erase Features- SacredGroveBoundary
 -Output Feature- Surrounding_Zone
This operation removes the sacred grove boundary from the 1-km buffer, producing a polygon representing the surrounding landscape outside the grove.
The resulting Surrounding_Zone is intended for separate assessment of surrounding industrial and anthropogenic pressures.
**Important analytical distinction**: NDVI and LULC analysis use the full 1-km buffer, including the sacred grove. The Surrounding_Zone is used when the analysis specifically requires exclusion of the grove itself.

**NDVI Analysis – 2017**
Software used: ArcGIS Pro
Satellite data: Sentinel-2
Spatial resolution: 10 metres
Normalized Difference Vegetation Index (NDVI) was calculated to assess vegetation greenness and spatial variation in vegetation conditions in study area.

**Satellite Band Selection**
Sentinel-2 bands used for NDVI calculation: Band4 (RED Spectral region, Resolution:10m, Purpose: Red Reflectance) & Band8 (near Infrared spectral region, Resolution: 10m, Purpose: Near-infrared reflectance)

**Clipping Satellite Bands**
