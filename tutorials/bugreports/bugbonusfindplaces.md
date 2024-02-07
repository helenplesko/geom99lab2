# Bug Report for Tutorial 3 (Bonus): Find places

## Describe the bug

The purpose of the ArcGIS Maps SDK for JavaScript "Find places" Tutorial is to create a map that allows you to see places on the map depending on the category chosen. It allows you to click the graphics as well, to find the name and address of the places in a pop-up. However, after completing the tutorial and opening the html page in Google Chrome, nothing appears.

## Steps to reproduce bug

The bug doesn't happen sporatically for me, it happens every time. Here are the steps to duplicating the bug:

1. Complete the ArcGIS Maps SDK for JavaScript ["Add a point, line, and polygon"](https://developers.arcgis.com/javascript/latest/tutorials/add-a-point-line-and-polygon/) Tutorial. Add API Key to code. Save the code in VSCode, then commit and push to the GitHub repository. 
2. Open the page URL in web browser.
3. Ctl+Shift+C to inspect page and see the errors.

## Expected result

The code in the tutorial is expected to display a map that allows you to see places on the map depending on the category chosen. It also allows you to click the graphics as well, to find the name and address of the places in a pop-up. Here is a screenshot taken from the tutorial page:

![Expected Result](/tutorials/bugimages/expectedbonusfindplaces.png)

## Results from the bug

The bug produced no map and two errors:

URL:
```
https://helenplesko.github.io/geom99lab2/tutorials/bonusfindplaces.html
```

![Errors](/tutorials/bugimages/bugbonusfindplaces.png)

## Attempts to debug

### Attempt 1: Comment out API key

The first attempt to debugging this was to comment out the API key, as there was an error retrieving authorization. This change didn't produce a map. Instead, a window popped up where I had to sign into AGOL to see the item. My login wasn't working, and I wondered if it was because we need to sign into Fleming organization when signing in to AGOL.

URL to map:
```
https://helenplesko.github.io/geom99lab2/tutorials/testpages/testonebonusfindplaces.html
```

![Attempt 1 results](/tutorials/bugimages/testonebonusfindplaces.png)

### Attempt 2: Use a different API Key

For the second attempt, I created a new API Key, without a referrer link this time, and here are the results:

URL to map:
```
https://helenplesko.github.io/geom99lab2/tutorials/testpages/testtwobonusfindplaces.html
```

![Attempt 2 results](/tutorials/bugimages/testtwobonusfindplaces.png)

## Environment Details

- VSCode was used to make, commit, and push changes to GitHub.
- Google Chrome is the web browser used to open maps.
- The problem is happening on my computer and on my iPhone.
- API Key was made in ArcGIS Developers.
- Referrer Link includes an * at the end.