# Bug Report for Tutorial 2: Add a point, line, and polygon

## Basemap error debugged!!!

When playing around with the basemaps for my customized map, an error had popped up saying the basemap name I chose was invalid. I noticed in the list of valid basemaps, "arcgis/topographic" wasn't there, but "topo" was. After looking more into these basemaps, "topo" is deprecated. So, I changed that line in the code to "topo-vector" and commented out my API Key and voila! The intended map was produced! 

Final URL: 
```
https://helenplesko.github.io/geom99lab2/tutorials/addpointlinepolygon.html
```

Basemap source: 
```
https://developers.arcgis.com/javascript/latest/api-reference/esri-Map.html#basemap
```

---

## Describe the bug

The purpose of the ArcGIS Maps SDK for JavaScript "Add a point, line, and polygon" Tutorial is to create a map that displays the topographic basemap layer for an area of the Santa Monica Mountains in California with point, line, and polygon graphics, plus a pop-up when the polygon is clicked. However, after completing the tutorial and opening the html page in Google Chrome, the graphics and pop-up appears, but the basemap doesn't.

## Steps to reproduce bug

The bug doesn't happen sporatically for me, it happens every time. Here are the steps to duplicating the bug:

1. Complete the ArcGIS Maps SDK for JavaScript ["Add a point, line, and polygon"](https://developers.arcgis.com/javascript/latest/tutorials/add-a-point-line-and-polygon/) Tutorial. Add API Key to code. Save the code in VSCode, then commit and push to the GitHub repository. 
2. Open the page URL in web browser.
3. Ctl+Shift+C to inspect page and see the errors.

## Expected result

The code in the tutorial is expected to display a map of the topographic basemap layer for an area of the Santa Monica Mountains in California with point, line, and polygon graphics, plus a pop-up when the polygon is clicked. Here is a screenshot taken from the tutorial page:

![Expected Result](/tutorials/bugimages/expectedaddpointlinepolygon.png)

## Results from the bug

The bug produced no map and two errors:

```
https://helenplesko.github.io/geom99lab2/tutorials/testpages/tutaddpointlinepolygon.html
```

![Errors](/tutorials/bugimages/bugaddpointlinepolygon.png)

## Attempts to debug

### Attempt 1: Comment out API key

The first attempt to debugging this was to comment out the API key, as there was an error retrieving authorization. This change didn't produce a map. Instead, a window popped up where I had to sign into AGOL to see the item. My login wasn't working, and I wondered if it was because we need to sign into Fleming organization when signing in to AGOL.

```
https://helenplesko.github.io/geom99lab2/tutorials/testpages/testoneaddpointlinepolygon.html
```

![Attempt 1 results](/tutorials/bugimages/testoneaddpointlinepolygon.png)

### Attempt 2: Use a different code

For the second attempt, I used the older version of the stylesheet, reference to ArcGIS, and basemaps. The code can be found in the "Display a map (2D)" tutorial. 

![Older version of code](/tutorials/bugimages/olderversioncode.png)

I used this code and it produced the following, which I believe is a closer result to what we want the map to display:

```
https://helenplesko.github.io/geom99lab2/tutorials/testpages/testtwoaddpointlinepolygon.html
```

![Attempt 2 results](/tutorials/bugimages/testtwoaddpointlinepolygon.png)

## Environment Details

- VSCode was used to make, commit, and push changes to GitHub.
- Google Chrome is the web browser used to open maps.
- The problem is happening on my computer and on my iPhone.
- API Key was made in ArcGIS Developers.
- Referrer Link for API Key includes an * at the end.