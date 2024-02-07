# Bug Report for Tutorial 1: Display a map

## Describe the bug

I used the code from the ArcGIS Maps SDK for JavaScript [Display a map](https://developers.arcgis.com/javascript/latest/tutorials/display-a-map/) Tutorial to create a map that displays the topographic basemap layer for an area of the Santa Monica Mountains in California. The code was saved in an html file on GitHub and when the page was visited, the map did not appear and there was an error with the basemap.

## Steps to reproduce bug

1. Complete the "Display a map" tutorial (linked above). Save the code in VSCode, then commit and push to the GitHub repository.
2. Open the page URL in web browser.
3. Ctl+Shift+C to inspect page and see the errors.

## Results expected

The code is expected to display a map that looks like this:

![Expected Result](/tutorials/bugimages/expecteddisplayamap.png)

## Results from the bug

The bug produced no map and two errors:

![Errors](/tutorials/bugimages/bugdisplayamap.png)

## Steps taken in attempt to resolve issue

### Attempt 1: Comment out API key

The first attempt to making this work was to comment out the API key, as adding a Referrer Link to the GitHub page was causing issues for others as well. However, when I did that, it didn't work. Instead, it was producing a window where I had to sign into AGOL to see the item, but my login wasn't working.

URL to map:
```
https://helenplesko.github.io/geom99lab2/tutorials/testonedisplayamap.html
```

![Attempt 1 results](/tutorials/bugimages/testonedisplayamap.png)

### Attempt 2: Use a different code

For the second attempt, I noticed that there were two different tutorials with similar names. One was ["Display a map"](https://developers.arcgis.com/javascript/latest/tutorials/display-a-map/) and the other was "Display a map (2D)", which was found on the API Key page that I created.

The "Display a map (2D)" tutorial used a different stylesheet, reference to ArcGIS, and basemaps. I used this code and it produced the following, which I believe is a closer result to what we want the map to display:

URL to map:
```
https://helenplesko.github.io/geom99lab2/tutorials/testtwodisplayamap.html
```

![Attempt 2 results](/tutorials/bugimages/testtwodisplayamap.png)

### Attempt 3: Copy code directly

Since I was following the steps of the tutorial and copying it piece by piece, I thought maybe I had missed a chunk of code. So, I copied and pasted the code directly from the last step in the tutorial, but the results produced the same errors as the original bug results.

## Environment Details

- VSCode was used to make, commit, and push changes to GitHub.
- Google Chrome is the web browser used to open maps.
- The problem is happening on my computer and on my iPhone.
- API Key was made in ArcGIS Developers.
- Referrer Link includes an * at the end.
