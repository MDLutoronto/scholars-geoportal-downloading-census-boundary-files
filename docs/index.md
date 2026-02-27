---
title: "Downloading census boundary files using Scholars GeoPortal"
layout: "home"
description: "This exercise will showcase how to use Scholars GeoPortal to extract Census Tract (CT) census geography for the Census Metropolitan Area (CMA) of Montreal using two methods: querying the attribute table of the dataset, or downloading based on a predefined census boundary (ex. CMAs)."
created_date: 2016-07-26
permalink: "/"  #! Remove this if not the homepage
---

# Downloading census boundary files using Scholars GeoPortal

This exercise will showcase how to use Scholars GeoPortal to extract Census Tract (CT) census geography for the Census Metropolitan Area (CMA) of Montreal using two methods:

1) querying the attribute table of the dataset, or

2) downloading based on a predefined census boundary (ex. CMAs).

1. Open Scholars GeoPortal by going to <http://geo.scholarsportal.info>
2. Use the main search box to search for census tract boundary files. You can search by phrase, keyword, title, and more.  
Type in the phrase “Census Tracts 2011” and click **Search**.  
<img src='{{ '/assets/images/2_searchbar.PNG' | relative_url }}' alt='Screenshot highlighting the search bar and search button in Scholars GeoPortal.' title='' width='680' height='412' />

3. As you hover over the search results a grey boundary will appear on the map; this represents the geographic coverage of the dataset.  
<img src='{{ '/assets/images/3_greyboundary.png' | relative_url }}' alt='Screenshot showing the grey boundary which represents the geographic coverage of the selected dataset.' title='' width='900' height='536' />

4. For this example we will work with Cartographic Boundary Files. Click **Add** to add the data to the map. If you want more information about the dataset you can click **Details**.  
  
    Note: You will notice two types of boundary files have been returned in the results: Cartographic Boundary Files (CBF) and Digital Boundary Files (DBF). Both are produced by Statistics Canada for the purposes of mapping the Census Geography. Cartographic boundary files depict the geographical areas using only the major land mass of Canada and its coastal islands. These files are good for creating thematic and choropleth maps. Digital boundary files depict the full extent of the geographical areas, including coastal water areas and boundaries.  
    <img src='{{ '/assets/images/4_addData.png' | relative_url }}' alt='Screenshot showing the location of the button to add a dataset to the map.' title='' width='532' height='416' />
5. After you click **Add** you will have to select the specific files you wish you add. For this example, add the file titled Census Metropolitan Areas & Census Agglomerations.  
<img src='{{ '/assets/images/5_addCMA.png' | relative_url }}' alt='Screenshot highlighting the specific file to add to the map.' title='' width='535' height='617' />

Option 1: Querying and filtering data for export
------------------------------------------------

1. After you’ve added data to the map, you can open the underlying data table (attribute table). You can access this table by clicking on the **Data Table** tab in the top right corner of the window.  
<img src='{{ '/assets/images/option1_1_datatable.png' | relative_url }}' alt='Screenshot showing the location of the Data Table button.' title='' width='757' height='171' />

2. The data table will open at the bottom of the page. You can scroll through the table using the blue arrows.  
<img src='{{ '/assets/images/option1_2_bluearrows.PNG' | relative_url }}' alt='Screenshot showing the location of the blue navigation arrows in the Data Table.' title='' width='900' height='328' />

3. Clicking on a feature in the table will highlight the feature on the map.  
Note: you can close the data table at any time by clicking on the **X** at the top right of the data table.  
<img src='{{ '/assets/images/option1_3_highlightfeature.PNG' | relative_url }}' alt='Screenshot showing a feature on the map which is highlighted after selecting the feature from the Data Table.' title='' width='855' height='473' />

4. You can query data to filter out results based on the fields in the data. To open the query **MENU** click on the **Query** button.  
<img src='{{ '/assets/images/option1_4_querybutton.PNG' | relative_url }}' alt='Screenshot showing the location of the Query button.' title='' width='514' height='244' />

5. For this example we are looking for the greater Montreal area, so we will filter using the CMAUID code. First, double click on **CMAUID: String**. Next, click on the equals symbol. These selections will appear in the query box to the right.  
<img src='{{ '/assets/images/option1_5_cmauid.PNG' | relative_url }}' alt='Screenshot showing the query selections.' title='' width='900' height='292' />

6. Click inside the query box to the right of the equals symbol in order to type the CMAUID code, which for Montreal is 462. Once you have typed in the CMAUID click **Execute**.  
<img src='{{ '/assets/images/option1_6_executequery.PNG' | relative_url }}' alt='Screenshot highlighting the custom query and the execute button.' title='' width='786' height='203' />

7. Once your query results are returned you can export by clicking on **Export Result**, then selecting **…as Shapefile**.  
<img src='{{ '/assets/images/option1_7_executequery.PNG' | relative_url }}' alt='Screenshot highlighting the export result tab and the shapefile selection.' title='' width='575' height='179' />

8. After the export runs you will be able to access your shapefile in the Download tab, or by clicking on the **Your file is available here** message which will appear at the top right of the data table.  
<img src='{{ '/assets/images/option1_8_fileavailable.PNG' | relative_url }}' alt='Screenshot highlighting the location of the Download tab and the File Available message.' title='' width='901' height='572' />

9. Click on the file to download and save to your computer.  
<img src='{{ '/assets/images/option1_9_zipfile.PNG' | relative_url }}' alt='Screenshot highlighting the .zip file which is ready for download.' title='' width='528' height='265' />

 

Option 2: Download data by a pre-defined census boundary
---------------------------------------------------------

1. Once the CMA data has been added to the map, click on the **Download** tab. Here you are given the option of downloading the entire dataset (which is typically a very large .zip file), downloading based on a pre-defined area (such as a province), or downloading based on an area you define by drawing an area on the map.  
<img src='{{ '/assets/images/option2_1_downloadtab.PNG' | relative_url }}' alt='Screenshot showing the two download options within Scholars GeoPortal.' title='' width='469' height='197' />

2. Since we want to download the Census Metropolitan Area of Montreal we will download by area of interest. First, select **Download by area of interest**, and then select **Select a pre-defined area**. Next, use the drop-down menu to select an area type, in this case Census Metropolitan Area (CMA).  
<img src='{{ '/assets/images/option2_2_predefinedarea.PNG' | relative_url }}' alt='Screenshot highlighting which buttons to select in order to select Census Metropolitan Areas as the pre-defined area type.' title='' width='472' height='415' />

3. Zoom and pan the map to find your desired area. When you find it, click on the desired area; this will highlight the area.  
<img src='{{ '/assets/images/option2_3_selectmontreal.PNG' | relative_url }}' alt='Screenshot showing the selected area which has been highlighted on the map.' title='' width='900' height='530' />

4. Select the desired output file format from the drop-down menu. To be able to use the file in ArcGIS select **Shapefile – (.shp)**.  
<img src='{{ '/assets/images/option2_4_fileformat.PNG' | relative_url }}' alt='Screenshot highlighting the correct output file format selection.' title='' width='470' height='596' />

5. Keep the output coordinate system as **Same as Input** (this defines the spatial reference system used to display your data).  
<img src='{{ '/assets/images/option2_5_outputcoordinate.PNG' | relative_url }}' alt='Screenshot highlighting the correct output coordinate system selection.' title='' width='471' height='341' />

6. Click **Download** to prepare the file for download. When the process is complete the .zip file will appear listed under the **My download list** section. Click on the file to download it to your computer.  
<img src='{{ '/assets/images/option2_6_download.PNG' | relative_url }}' alt='Screenshot showing the locations of the Download button and the .zip file which is ready to be downloaded.' title='' width='466' height='276' />

 

 [Downloading_Census_Boundary_Files_Using_ScholarsGeoPortal.pdf](https://mdl.library.utoronto.ca/sites/default/public/Downloading_Census_Boundary_Files_Using_ScholarsGeoPortal.pdf)
 
 Technique: [Searching for maps and data](https://mdl.library.utoronto.ca/technique/searching-maps-and-data) | Data Format: [Vector](https://mdl.library.utoronto.ca/data-format/vector)
