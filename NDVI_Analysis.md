Go to ArcGIS and under add data import the Bands B02, B03, B04, and B08.
Go to tools under analysis and search for composite bands. Combine all the bands to display colour images and run vegetation analysis.

Verify the 26-hectare grove boundary
To analyze the impact of industial pollution surrounding the sacred grove boundary within 1000m radius we need to erase the Shivbari Grove boundary feature:
Analysis → Tools → Erase
Input Features: 1-km buffer
Erase Features: Shivbari grove boundary
Output: Surrounding_Zone
<img width="1134" height="237" alt="Screenshot 2026-11-16 213203" src="https://github.com/user-attachments/assets/e4212768-5a61-43fb-97cd-8b5ff94213db" />

We need to do NDVI analysis and LULC Chnage analysis only withing the 1000m buffer therefore in the next step we will Clip the satellite imagery-
Go to analysis-tools-clip raster
<img width="1182" height="821" alt="Screenshot 2026-11-23 105039" src="https://github.com/user-attachments/assets/4b84b46b-dfd7-48a1-b42d-6d6159c006aa" />
Follow this step for other bands as well.
