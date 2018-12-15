# LineNavigation
This is a Project for the course of Future User Interface

## Motivation
While mobile navigation is omnipresent outdoors, it is not inside buildings because of the normally non-existent GPS reception. Wi-Fi is often used in this case to create a so-called “indoor GPS”. However, its accuracy is 5-15 meters and iOS devices are excluded from client-based positioning. Beacons are the alternative, which have accuracy of 1-3 meters, while interference can occur when beacons are installed in a space with lots of Wi-Fi signals.

In order to make a high accuracy, low cost and easy plug-in system, we decide to use computer vision technology, with Augmented Reality lines guiding the ways. This app is for indoor places such as a hall, a library, parking garage and subway transit system. The more people use the app, create the routes and voted for the popular routes, the more well-established the system will be.

## Implementation
### Frontend: Android
We forked the code of 'Just a Line" and added many new interfaces. Currently it supports recording a route with only two labels. Search a route with route number or 

### Backend: Django
We design the backend to receive a route with many labels and form a complete map and generate routes between any two labels automatically. The algorithm to find the shortest path among any two points has been implemented but still unused.

## Future Work
### Support 3D route
It is easy to support this feature with raw route, but it is a little difficult to calculate a 3D map.
### Support Map Combination
Currently our backend doesn't support map combination but this is within our consideration when we design the data structure of map. 
### Input multi labels when recording the route
Currently we can only type two labels when we record the route. We need to customize the widget of ListView of android to support this feature.
### Detect building automatically
In the future, we don't need the user to type the building name manually because we can locate the user's place through GPS and type it automatically. Unless it is wrong, user can modify it manually. 
