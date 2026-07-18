#### Downloaded Data. 
- We Get the following datasets from the National Historical Geographic Information System (NHGIS): (https://data2.nhgis.org/main)
	- total population (blockgroup-level) for 2019.
	- Shapefiles 2010 (block-level) for Boston and Philly. We use 2010 as it's the most recent census year matching the 2019 identifier.

- We Get the following dataset from the US Census: (https://data.census.gov) 
	- Median income `B19013` (blockgroup-level) for 2019 for Boston and Philly.  

#### Queried Data. 
`..\Code\ A_DataCollection.ipynb` queries the following data: 
- Use OpenStreetMap (OSM) API to draw coordinates of residential areas (`Tag:landuse=residential`) in Boston and Philly 
- Use Google StreetView Static API to query multi-angled street images (0°, 90°, 180°, 270°) for a randomly selected list of locations. 
- Use the US census API to construct: 
	- Income (`B19013_001E`)
	- Home Value (`B25077_001E`)
	- Vacancy Share (`B25002_003E`/`B25002_001E` )
	- Higher Education Share ((`B15003_022E` + `B15003_023E` + `B15003_024E` + `B15003_025E`)/`B15003_001E`)


#### Links to Data Folders. 
- **Input:** https://drive.google.com/drive/folders/1KV1sFrXFUBdA9YEbUWW3SZeaVVq5D0Lx?usp=share_link
- **Output:** https://drive.google.com/drive/folders/12hMDvf96tO774b7cXkmaiyaKKDJyLt8i?usp=share_link
