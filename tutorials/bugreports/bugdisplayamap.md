# Bug Report for Tutorial 1: Display a map

## Describe the bug

The purpose of the ArcGIS Maps SDK for JavaScript "Display a map" Tutorial is to create a map that displays the topographic basemap layer for an area of the Santa Monica Mountains in California. However, after completing the tutorial and opening the html page in Google Chrome, the map appeared blank and there was an error with the API Key and the basemap.

## Steps to reproduce bug

The bug doesn't happen sporatically for me, it happens every time. Here are the steps to duplicating the bug:

1. Complete the ArcGIS Maps SDK for JavaScript ["Display a map"](https://developers.arcgis.com/javascript/latest/tutorials/display-a-map/) Tutorial. Add API Key to code.Save the code in VSCode, then commit and push to the GitHub repository. 
2. Open the page URL in web browser.
3. Ctl+Shift+C to inspect page and see the errors.

## Expected result

The code in the tutorial is expected to display a map that displays the topographic basemap layer for an area of the Santa Monica Mountains in California. Here is a screenshot taken from the tutorial page:

![Expected Result](/tutorials/bugimages/expecteddisplayamap.png)

## Results from the bug

The bug produced no map and two errors:

```
https://helenplesko.github.io/geom99lab2/tutorials/testpages/tutdisplayamap.html
```

![Errors](/tutorials/bugimages/bugdisplayamap.png)

## Environment Details

- VSCode was used to make, commit, and push changes to GitHub.
- Google Chrome is the web browser used to open maps.
- The problem is happening on my computer and on my iPhone.
- API Key was made in ArcGIS Developers.
- Referrer Link for API Key includes an * at the end.

## Attempts to debug

### Attempt 1: Comment out API key

The first attempt to debugging this was to comment out the API key, as there was an error retrieving authorization. This change didn't produce a map. Instead, a window popped up where I had to sign into AGOL to see the item. My login wasn't working, and I wondered if it was because we need to sign into Fleming organization when signing in to AGOL.

```
https://helenplesko.github.io/geom99lab2/tutorials/testpages/testonedisplayamap.html
```

![Attempt 1 results](/tutorials/bugimages/testonedisplayamap.png)

### Attempt 2: Use a different code

For the second attempt, I noticed that there were two different tutorials with similar names. One was ["Display a map"](https://developers.arcgis.com/javascript/latest/tutorials/display-a-map/) and the other was "Display a map (2D)", which was found on the API Key page that I created.

The "Display a map (2D)" tutorial used an older version of the stylesheet, reference to ArcGIS, and basemaps. 

![Older version of code](/tutorials/bugimages/olderversioncode.png)

I used this code and it produced the following, which I believe is a closer result to what we want the map to display:

```
https://helenplesko.github.io/geom99lab2/tutorials/testpages/testtwodisplayamap.html
```

![Attempt 2 results](/tutorials/bugimages/testtwodisplayamap.png)

### Attempt 3: Comment out API Key and change the basemap

When playing around with the basemaps for my customized map, an error had popped up saying the basemap name I chose was invalid. I noticed in the list of valid basemaps, "arcgis/topographic" wasn't there, but "topo" was. After looking more into these basemaps, "topo" is deprecated. So, I changed that line in the code to "topo-vector" and commented out my API Key and voila! The intended map was produced! API Key remained commented out.

Final URL: 
```
https://helenplesko.github.io/geom99lab2/tutorials/displayamap.html
```

Basemap source: 
```
https://developers.arcgis.com/javascript/latest/api-reference/esri-Map.html#basemap
```

## Conclusion

- API Key still didn't work - had to remain commented out
- Basemap "arcgis/topographic" was not recognized, had to change to "topo-vector"