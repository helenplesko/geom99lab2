# ArcGIS Online and GeoJSON

## Task 1:

Using your saved GeoJSON file, now import it into your ArcGIS Online account and create an ArcGIS Online WebMap displaying it. 

### Method:

1. The polygon points were plotted using https://geojson.io/. 
2. The JSON code was copied into Notepad++ and saved as a GeoJSON file with the extension .geojson. 
3. In AGOL, this GeoJSON file was added from my device via the New Item button on the Content page, and it was added with a hosted feature layer. 
4. This feature layer was then opened up in Map Viewer and saved as a Web Map. 

---

## Task 2 (Bonus):

Can you store your GeoJSON in GitHub and display it on the ArcGIS Map Viewer? 

### Method:

1. A copy of the GeoJSON file from Task 1 was added to GitHub.
2. In Map Viewer, via the Contents toolbar, the GeoJSON file was added from URL ("Add">"Add layer from URL"). Two layers were created.
```https://helenplesko.github.io/geom99lab2/geojson/capybarasgithub.geojson```
    - 1st Layer: "Create a hosted feature layer and add it to the map"
    - 2nd Layer: "Reference the file from the URL and add it to the map"

### Question: 

What happens if you make a change to the file in GitHub?

### Answer:

After the layers were added to a new map following the method above, I went into GitHub and deleted the first polygon feature in the GeoJSON file. After reopening the Map with the two layers, only the layer that referenced the file from the URL showed a change in the data. The data hosted as a feature layer, did not change. This result is shown in the image below:

![After edit was made in GitHub](/geojson/geojsonimages/aftergithubedit.png)

Only the layer that references the URL was affected because the data is pulled and loaded from the URL every time the map is opened. Whereas, the data in the hosted feature layer is managed completely within AGOL and references the GeoJSON file stored in AGOL instead, which was unchanged.

---

## Question:

Given the method you used to add it to ArcGIS Online, where and how is your actual GeoJSON data stored? Don't guess! Show your work for each type you used, including the bonus above.

## Answer:

For the hosted feature layers, the GeoJSON data is stored in the GeoJSON file on AGOL. 

Task 1

![Task 1 hosted feature layer and geojson](/geojson/geojsonimages/hostedfeaturelayerfilesone.png)

Task 2

![Task 2 hosted feature layer and geojson](/geojson/geojsonimages/hostedfeaturelayerfilestwo.png)

The GeoJSON files are published as the feature layer, as shown in the details of both files

Task 1

![Task 1 hosted feature layer details](/geojson/geojsonimages/hostedfeaturelayerdetailsone.png)

![Task 1 geojson details](/geojson/geojsonimages/geojsondetailsone.png)

Task 2

![Task 2 hosted feature layer details](/geojson/geojsonimages/hostedfeaturelayerdetailstwo.png)

![Task 2 geojson details](/geojson/geojsonimages/geojsondetailstwo.png)

The layer in the github map from Task 2, that references the URL, is directly linked to the data stored in the geojson file on GitHub.

![Task 2 geojson details](/geojson/geojsonimages/geojsondetailstwo.png)