# A-Frame and D3.js

The A-Frame library may be used as a WebVR rendering layer for D3.js. A-Frame and D3 "meet" at the DOM level. D3 may be used to create and dynamically modify any of A-Frame's primitive elements inside of an a-scene.

A-Frame and D3.js are not yet perfectly compatible. Specifically, updating properties of a custom component that has multiple attributes is difficult. Neither '.attr()' or '.property()' work as-is for this task. One option is to parse and then re-construct the entire attribute string for your component, but this may be slow. D3 could be modified to better support A-Frame by exposing a method that modifies a component attribute of each element in a selection. 

In this demo a collection of a-box elements are created and used to display some random data. You may use the floating button to randomly create a new set of data. D3 updates the boxes with the new data when this happens.

[View this demo on GitHub Pages](https://mikebolt.github.io/aframe-d3-demo/)
