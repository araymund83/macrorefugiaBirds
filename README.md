#Macrorefugia Indices for North American Avifauna
##Data description:
Velocity-based macrorefugia metrics for 400 North American breeding bird species were developed for two future time periods (2041-2070, 2071-2100) and three global climate models (GCMs: CCSM3, GFDLCM3, INMCM4) based on species distribution model projections by Bateman et al. (2020) and using the approach described in Stralberg et al. (2018). Individual species projections based on GCM ensembles are available for viewing at https://www.audubon.org/climate/survivalbydegrees and raster files can be downloaded from Adaptwest (https://adaptwest.databasin.org/pages/audubon-survival-by-degrees/).
Backward biotic velocity (Carroll et al., 2015) for each species was calculated using the nearest-analog velocity algorithm defined by Hamann et al. 2015 and applied to binary presence/absence rasters representing current and projected future distributions. Presence thresholds were based on mean probability of occurrence in the baseline period. To convert biotic velocity into an index of microrefugia ranging from 0 to 1, a distance-decay function was applied to the backward velocity distance valuer at each pixel, i.e., the shortest distance from a projected future location to the current distribution. The distance-decay function was based on a fat-tailed distribution (c= 0.5, and alpha = 8333.33) parameterized to result in a mean migration rate of 500 m/year or 50 km/century (details in Stralberg et al. 2018). Refugia index values were calculated separately for each GCM and then averaged to produce an overall index.
Code (updated from Stralberg et al. 2018) is available at:  https://doi.org/10.5281/zenodo.14680928
Macrorefugia indices are provided as GeoTIFFs with a 1-km resolution and projection, with map images provided in png format. All data layers are in the Albers Conic Equal Area projection (EPSG: 102008). The values of the index have been multiplied by 100 to create smaller integer files. Indices for individual species have been combined by habitat types following Bateman et al. (2020). Species groups available for download are: 
Arctic, Aridlands, Boreal Forest, Coastal, Eastern Forest, Generalists, Grasslands, Marshlands, Subtropical, Urban, Waterbirds and Western Forest

##Files are named as follows: 
Spp_refugia_X_ Y
where: 
Spp = bird species four-letter code
X = Representative Concentration Pathway (4.5 or 8.5)
Y = year (2025, 2055, 2085)

##Projection information 
Project Coordinate System: Albers_Conic_Equal_Area
Linear Unit: Meters
False Easting: 0.0
False Northing: 0.0
Central Meridian: -96.0
Standard parallel 1: 20.0
Standard parallel 2: 60.0
Latitude of origin:  40.0
Cell size: 1000

##References
Bateman, B. L., Wilsey, C., Taylor, L., Wu, J., LeBaron, G. S., & Langham, G. (2020). North American birds require mitigation and adaptation to reduce vulnerability to climate change. Conservation Science and Practice, 2(8), e242. https://doi.org/10.1111/csp2.242
Carroll, C., Lawler, J. J., Roberts, D. R., & Hamann, A. (2015). Biotic and Climatic Velocity Identify Contrasting Areas of Vulnerability to Climate Change. PLOS ONE, 10(10), e0140486. https://doi.org/10.1371/journal.pone.0140486
Hamann, A., Roberts, D. R., Barber, Q. E., Carroll, C., & Nielsen, S. E. (2015). Velocity of climate change algorithms for guiding conservation and management. Global Change Biology, 21(2), 997–1004. https://doi.org/10.1111/gcb.12736
Stralberg, D., Carroll, C., Pedlar, J. H., Wilsey, C. B., McKenney, D. W., & Nielsen, S. E. (2018). Macrorefugia for North American trees and songbirds: Climatic limiting factors and multi-scale topographic influences. Global Ecology and Biogeography, 27(6), 690–703. https://doi.org/10.1111/geb.12731
