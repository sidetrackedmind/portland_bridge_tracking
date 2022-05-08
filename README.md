# portland_bridge_tracking
use google location history data to figure out if I crossed all of Portland's bridges.

## Google Location History
Using the google Timeline UI, I can see all the trips I've made. Depending on how many location pings were collected, it's possible to see which bridges I crossed on a given trip:
![image](https://user-images.githubusercontent.com/24400820/167315554-729f9376-3ac4-4f3d-893a-f24fe5da8716.png)

## Google Takeout
Instead of searching through the UI for all the times I crossed a bridge. My plan is to download my location data from [Google Takeout](https://takeout.google.com/settings/takeout). It's possible to download all the location data as a .zip json.

## Plan

1. Download all location data
2. Find Portland bridge GIS files (ideally from City of Portland)
3. Buffer portland bridges by some amount (let's start with 500 m)
4. Clip all location pings within the bridge buffers
5. See if I captured all bridges

