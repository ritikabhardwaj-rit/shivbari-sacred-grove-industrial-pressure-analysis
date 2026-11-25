Go to ArcGIS and under add data import the Bands B02, B03, B04, and B08.
Go to tools under analysis and search for composite bands. Combine all the bands to display colour images and run vegetation analysis.

Verify the 26-hectare grove boundary
Clip the satellite imagery to the 1-km buffer surrounding the sacred grove to restrict the analysis to the defined study area:
Analysis → Tools → Erase
Input Features: 1-km buffer
Erase Features: Shivbari grove boundary
Output: Surrounding_Zone
<img width="1134" height="237" alt="Screenshot 2026-11-16 213203" src="https://github.com/user-attachments/assets/e4212768-5a61-43fb-97cd-8b5ff94213db" />

We need to do NDVI analysis and LULC Chnage analysis only withing the 1000m buffer therefore in the next step we will Clip the satellite imagery-
Go to analysis->tools->clip raster
<img width="1182" height="821" alt="Screenshot 2026-11-23 105039" src="https://github.com/user-attachments/assets/4b84b46b-dfd7-48a1-b42d-6d6159c006aa" />
Follow this step for other bands as well.

NDVI subsequently calculated to examine the spatial variation in vegetation greenness. Now calculate NDVI: Go to analaysis->tools->Raster calculation
(The Normalized Difference Vegetation Index (NDVI) was calculated using the following equation:
NDVI = (NIR − Red) / (NIR + Red)

Where:
NIR represents Band 8 (Near Infrared).)
Red represents Band 4 (Red).

<img width="1061" height="805" alt="Screenshot 2026-11-23 113934" src="https://github.com/user-attachments/assets/e2a8c42d-23e8-4699-8a19-6e3a6bcf31e0" />
Change the NDVI colour scheme:
In Contents, right-click RasterC_1.-Select Symbology-Keep Primary Symbology as Stretch-Find the Color scheme dropdown-Select a colour ramp that progresses from brown/yellow to green
Figure: NDVI distribution across Shivbari Sacred Grove and its surrounding 1-km landscape, derived from Sentinel-2 imagery acquired on 12 February 2017.
<img width="580" height="403" alt="Screenshot 2026-11-23 173724" src="https://github.com/user-attachments/assets/6fc61349-6615-4af8-84ef-e0a1a1e730fa" />

Map Interpretation:
The NDVI output indicates spatial variations in vegetation greenness across the sacred grove and its surrounding landscape.
The sacred grove boundary exhibits predominantly green and yellow-green pixels, while the surrounding landscape displays a more heterogeneous pattern, with patches of varying NDVI values.
The calculated NDVI values range from approximately -0.010 to 0.640. These variations provide an initial indication of differences in vegetation greenness and surface characteristics across the study area.

Relevance to the Study:
This analysis establishes a baseline for assessing vegetation conditions within Shivbari Sacred Grove in relation to its surrounding industrialising landscape, where 16 industrial units have been identified within a 1-km radius.
The 2017 NDVI assessment will serve as a reference for comparison with 2026 Sentinel-2 imagery to investigate changes in vegetation greenness over time.
