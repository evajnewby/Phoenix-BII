# Biodiversity Intactness Index (BII) Change in Phoenix, Arizona

Author: Eva Newby (https://github.com/evajnewby)

## About
The following repository was created for edicational purposes for EDS 220 - Working with Environmental Datasets, for the Masters of Environmental Data Science program at the Bren School of Environmental Science and Management at the University of California, Santa Barbara. 

In 2021, Maricopa County, which includes the Phoenix metropolitan area, was recognized as the U.S. county with the largest increase in developed land since 2001 [1]. This rapid urban expansion has significant implications for biodiversity and the health of nearby natural ecosystems.

The analysis in the `phoenix_biodiversity.ipynb` aims to explore the changes in BII within the Phoenix County subdivision area from 2017 to 2020, highlighting the impact of urban growth on biodiversity over time. To achieve this, the notebook contains code to create a map of the Phoenix subdivision in its broader geographic context, calculate the percentage of the subdivision's area with a BII of at least 0.75 in both 2017 and 2020, and develop a visualization to illustrate the area with a BII ≥ 0.75 in 2017 that was lost by 2020.

The `data` folder contains all necessary data for the analysis, including shapefiles for the state of Arizona accessed through the US Census Bureau Website. 

## Highlights
- Access data from the Microsoft Planetary Computer STAC Catalog
- Wrangling vector and raster data
- Plotting raster data
- Summing pixel data 

## Data
The BII data was accessed from the Microsoft Planetary Computer STAC Catalog. The code in this notebook contains steps to access the catalog for the correct location and dates. 

The Arizona shapefile was accessed from the US Census Bureau's TIGER shapefiles. The code in this notebook contains steps to filter to the Phoenix area only. 

## Repository Structure
```bash
Phoenix-BII
├── README.md
├── .gitignore
├──  data
│     ├── tl_2020_04_cousub.cpg
│     ├── tl_2020_04_cousub.dbf
│     ├── tl_2020_04_cousub.prj
│     ├── tl_2020_04_cousub.shp
│     ├── tl_2020_04_cousub.shx
│     ├── tl_2020_04_cousub.shp.ea.iso.xml
│     ├── tl_2020_04_cousub.shp.iso.xml
│  
└── phoenix_biodiversity.ipynb

```

## References
F. Gassert, J. Mazzarello, and S. Hyde, “Global 100m Projections of Biodiversity Intactness for the years 2017-2020 [Technical Whitepaper].” Aug. 2022. Available: [https://ai4edatasetspublicassets.blob.core.windows.net/assets/pdfs/io-biodiversity/Biodiversity_Intactness_whitepaper.pdf]

Microsoft. IO Biodiversity Dataset. Planetary Computer. Retrieved from [https://planetarycomputer.microsoft.com/dataset/io-biodiversity]

University of California, Santa Barbara. (2024). EDS 220 - Working with Environmental Datasets. Retrieved from [https://meds-eds-220.github.io/MEDS-eds-220-course/]

U.S. Census Bureau. (2020). 2020 Census County Subdivisions Shapefiles. U.S. Department of Commerce. Retrieved from [https://www.census.gov/cgi-bin/geo/shapefiles/index.php?year=2020&layergroup=County+Subdivisions]

Z. Levitt and J. Eng, “Where America’s developed areas are growing: ‘Way off into the horizon’,” The Washington Post, Aug. 2021, Available: [https://www.washingtonpost.com/nation/interactive/2021/land-development-urban-growth-maps/]. [Accessed: Nov. 22, 2024]
