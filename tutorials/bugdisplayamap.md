# Bug Report for Tutorial 1: Display a map

## Describe the bug

I used the code from the ArcGIS Maps SDK for JavaScript [Display a map](https://developers.arcgis.com/javascript/latest/tutorials/display-a-map/) Tutorial to create a map that displays the topographic basemap layer for an area of the Santa Monica Mountains in California. The code was saved in an html file on GitHub and when the page was visited, the map did not appear and there was an error with the basemap.

## Steps to reproduce bug

1. Complete the "Display a map" tutorial (linked above)
2. Open the 

## Results expected

The map is expected to display a map that looks like this:


## Results from the bug


## Steps taken in attempt to resolve issue

### Attempt 1: Comment out API key

The first attempt to making this work was to comment out the API key, as adding a Referrer Link to the GitHub page was causing issues for others as well. However, when I did that, it didn't work. Instead, it was producing a window where I had to sign into AGOL to see the item, but my login wasn't working.

### Attempt 2: Use a different code

For the second attempt, I noticed that there were two different tutorials with similar names. One was ["Display a map"](https://developers.arcgis.com/javascript/latest/tutorials/display-a-map/) and the other was "Display a map (2D)", which was found on the API Key page that I created.

The "Display a map (2D)" tutorial used a different stylesheet and reference to ArcGIS. I replaced the two lines from the other tutorial with these dow

### Attempt 3: Copy code directly

Since I was following the steps of the tutorial and copying it piece by piece, I thought maybe I had missed a chunk of code. So, I created a new file

## Environment Details

I'm using VSCode to make, commit, and push changes to GitHub.
GitHub is open on Google Chrome.
The problem is happening on my computer and on my iPhone.
