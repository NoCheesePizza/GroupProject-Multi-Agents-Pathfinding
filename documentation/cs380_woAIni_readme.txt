Team: wo AI ni


Members Name: Alexis Tan Bing Rui, Brandon Ho Jun Jie, Clifford Tan Eng Kiat, George Koh Jia Hao


Description:

This simulation allows the user to visualize how NPCs explore intricate, obstacle-laden, and procedurally  generated maps. By combining various vector fields such as a distance-based heat map, a repulsion field, and a potential map, we are able to create NPCs that can pathfind through unknown environments in a realistic manner.


Notes:

- There is a minimap on the top right hand corner that does not display vector field colors
- Setting the map size to too large a number (e.g. width/height more than 75) may cause the simulation to lag
- The potential field does not currently take into account walls, so it should only be used on an empty map
- We only have one entity type, Enemy, so we will be using the terms "entity" and "Enemy" interchangeably
- There is 176 bytes of memory leak due to some issue with the SFML Window class and we are unable to fix it


Controls:

- Press Left Control + slide Vertical Scroll Wheel to zoom in and out
- Press W, A, S, D to move camera around
- All other parameters can be controlled by the ImGui panels on the left
- Left or right clicking will trigger various events depending on the draw mode (None, Wall, Goal, Entity) that can be set in the Map Maker
- Press F11 to toggle fullscreen

Draw Modes
----------
- None: Clicking does nothing, but walls are hidden until explored
- Wall: Left clicking and dragging adds walls at the cursor
- Wall: Right clicking and dragging removes walls at the cursor
- Goal: Left clicking starts exploration (does not need a goal, and Enemies will stop exploring once all accessible cells are explored)
- Goal: Right clicking adds the goal at the cursor (can only have 1 goal, and Enemies will go to the goal once it has been found)
- Entity: Left clicking adds an Enemy at the cursor
- Entity: Right clicking removes an Enemy at the cursor


Editor Windows:

Inspector
---------
- View and modify almost all of the variables of each entity

Control Panel
-------------
- Pause and resume the game
- Draw vision radius, heat map, and flow field
- Modify all Enemies' field of view
- Modify and draw the repulsion field
- Modify and draw the potential field

Map Maker
---------
- Load, save, save as, delete, and rename maps
- Clear things on the map, adjust the map size, and change the draw mode
- Set parameters for the procedural map generator


Main Menu
---------
- View the FPS
- Toggle the other windows


Our experience working on this project:

It has been fun working together on the engine and the algorithms. We had a dedicated leader who would assign jobs, call for meetings, and check on our work. All of us were tasked with vastly different features so that we wouldn't need to depend on one another to progress, and it was exciting to see them all come nicely together towards the end of the project. While we had our fair share of bugs that we couldn't fix for the submission, such as our potential field not working with walls, all of us have definitely learnt a lot from researching and implementing what we were tasked with. All in all, the project went quite smoothly as all of us had a similar work ethic, although we did have to change our research question a few times because of scoping issues. However, one thing that annoyed us was how we had to stay up until very late to rush the presentation and research paper, as we had been too bogged down by the many assignments from our other 3 modules to make much progress before the weekend of the submission.