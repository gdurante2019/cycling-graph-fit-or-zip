# Code for producing cycling workout summary graph
This repo houses updated code for a Streamlit-hosted app that takes in either a .fit file or a .zip of a fitfile and returns a graph with a similar color scheme to Zwift workout summary graphs.  The app's link will be posted once testing is completed.

_Note:_  these graphs are created from .fit files from any workout, whether on Zwift or not; no Zwift branding is implied and this effort is not connected to Zwift.  It's just a way for Zwift enthusiasts to compare workouts (even those from outdoor rides!) quickly.  

## Purpose
The inspiration for this project comes from discussions with fellow cycling enthusiasts who race in the Zwift Racing League on the Backpedal  (BAKPDL) team and would like to share their workout summary graphs from indoor trainer rides or outdoor rides in a simple, standardized way in chat discussions.  The utility of generating graphs in this format is to make it easy for community members to understand, at a glance, the workout efforts of their teammates and fellow cyclists.

## Usage
Users will upload workout fitfiles and enter their FTP. The resulting graph will contain smoothed power output, workout zones, a plot of heart rate during the workout, and max power and max heart rate annotations. Here's an example:

![image](https://github.com/gdurante2019/graph-workout-streamlit/blob/main/example_workout_graph.png)


## Acknowledgments
Many thanks to the following, whose code has helped enable this project!
* Johannes Jacob, whose blog provides code and instructions for converting .fit files into a pandas dataframe (http://johannesjacob.com/analyze-your-cycling-data-python/)
* David Cooper, who created the fitparse library (https://github.com/dtcooper/python-fitparse) referenced in Johannes Jacob's blog
* Jonas Häggqvist (https://github.com/rasher), fellow Backpedaler, who provided the smooth.py code for smoothing the workout data
* Phil Daws (https://github.com/vegancodecruncher), Vegan Triathlete and fellow Backpedaler, who provided starter code for adding artists to matplotlib plot
