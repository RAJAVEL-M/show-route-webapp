# show-route-webapp
find route between locations by mouse click on map 

Description:

A map which can be viewed as a web page where users can select locations in a mouse click or touch, it sends coordinates to a route finding API and draws route in the map.
For showing map leaflet a javascript library is used and the server is made using Django framework in python. when user click on a location it reversecode the location into coordinate and send to the route API.
The response is in the polyline encoded format and using python's polyline library we decode the response and fetch coordinates.
after fetching the coordinates are drawn in the map and shown it to the user.

Deployment:

The web app is deployed in Azure app service.
Open App service in azure. select resource group and give name, location, etc.
select deployment slots tab and select from Github project.
The selected source code is deployed using Github actions.
