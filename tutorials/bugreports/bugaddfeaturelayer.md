# Bug Report for Tutorial 3 (Bonus): Add a feature layer

## Describe the bug

The purpose of the ArcGIS Maps SDK for JavaScript "Add a feature layer" Tutorial is to create a map that uses URLs to access three hosted feature layers and displays them on the topographic basemap layer for an area of the Santa Monica Mountains in California. However, after completing the tutorial and opening the html page in Google Chrome, the map appeared blank and there was an error with the API Key, basemap, and accessing the feature layers.

## Steps to reproduce bug

The bug doesn't happen sporatically for me, it happens every time. Here are the steps to duplicating the bug:

1. Complete the ArcGIS Maps SDK for JavaScript ["Add a feature layer"](https://developers.arcgis.com/javascript/latest/tutorials/add-a-feature-layer/) Tutorial. Add API Key to code. Save the code in VSCode, then commit and push to the GitHub repository. 
2. Open the page URL in web browser.
3. Ctl+Shift+C to inspect page and see the errors.

## Expected result

The code in the tutorial is expected to display a map that displays the topographic basemap layer for an area of the Santa Monica Mountains in California. Here is a screenshot taken from the tutorial page:

![Expected Result](/tutorials/bugimages/expectedbonusaddfeaturelayer.png)

## Results from the bug

The bug produced no map and two errors:

```
https://helenplesko.github.io/geom99lab2/tutorials/testpages/tutbonusaddfeaturelayer.html
```

![Errors](/tutorials/bugimages/bugbonusaddfeaturelayer.png)

## Environment Details

- VSCode was used to make, commit, and push changes to GitHub.
- Google Chrome is the web browser used to open maps.
- The problem is happening on my computer and on my iPhone.
- API Key was made in ArcGIS Developers.
- Referrer Link for API Key includes an * at the end.

## Attempts to debug

### Attempt 1: Comment out API key and change basemap

Due to the errors occuring on the previous two tutorials as well, I jumped right to commenting out the API Key and changing the basemap from "arcgis/topographic" to "topo-vector". This made all feature layers appear, as well as the topographic basemap.

Final URL: 
```
https://helenplesko.github.io/geom99lab2/tutorials/displayamap.html
```

Basemap source: 
```
https://developers.arcgis.com/javascript/latest/api-reference/esri-Map.html#basemap
```

## Conclusion: 

- API Key still didn't work - had to remain commented out
- Basemap "arcgis/topographic" was not recognized, had to change to "topo-vector"

