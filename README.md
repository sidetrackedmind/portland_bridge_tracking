# Portland Bridge Tracking Background
Someone asked me recently if I had traveled over all the bridges in Portland going over the Willamette River. I couldn't remember off the top of my head but I know that I've been allowing google to track my location (for funsies) so maybe I could use that data to my advantage. This project is a test to see if I can use my google location history data to figure out whether I crossed all of Portland's bridges.

## Google Location History
Using the google Timeline UI, I can see all the trips I've made. Depending on how many location pings were collected, it's possible to see which bridges I crossed on a given trip:
![image](https://user-images.githubusercontent.com/24400820/167315707-5d48a083-c56f-4b37-8148-41d715bb1dc8.png)

## Google Takeout
Instead of searching through the UI, it's possible to download location data from [Google Takeout](https://takeout.google.com/settings/takeout) as a .zip json.

## Plan

1. Download all location data
2. Find Portland bridge [GIS files](https://gis-pdx.opendata.arcgis.com/datasets/river-bridges/explore?location=45.487463%2C-122.625796%2C11.53) or create bridge files (get_bridge_paths.ipynb)
3. Buffer portland bridges by some amount (let's start with 150 m)
4. Clip all location pings within the bridge buffers
5. See if I went over all the bridges (bonus see if Google data can tell me whether I drove, biked, or walked over the bridge)

