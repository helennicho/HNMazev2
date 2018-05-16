# A Maze Starter Project

This project is part of [Udacity](https://www.udacity.com "Udacity - Be in demand")'s [VR Developer Nanodegree](https://www.udacity.com/course/vr-developer-nanodegree--nd017).

## Versions
- Unity 2017.3.1f1
- GVR Unity SDK v1.70.0

Designing & Building the Maze
-----------------------------------
After some researh, I decided to build the maze manually rather than using an algorithm. However I did learn about the complexities of maze design and the the complexities of creating & using a maze algorith
The advantages of a manual design is that the layout and positioning of walls & objects can be better controlled thus allowing the maze design to be more appropriate for the target user type.
Also it means that lights and the maze layout are part of the static design to optimise performance.
I found it a fascinating learning experience though quite time consuming.
I used the complex set of prefabs (as provided) as a block design that I duplicated, re-positioned & rotated to create a grid. Then I deleted blocks to create a route through the maze to the Temple. Finally more blocks were created to create cul-de-sac routes around the maze.
I had to create end pillars as extra blocks to give a finished edge to some walls.
The main problem was it is difficult to get the lines of walls & cross pillars to line up exactly by hand but in the end I thought it gave a more rustic look and I made various "wall repairs" as I went along!

Maze Layout
---------------
The game starts with an overview of the Temple Maze floating in a rural settiing. User Interfaes (canvasses) are used to guide the less experienced user. 
Fixed user interfaces explain the navigation system (waypoints), how to collect items (look and click) and the final completion canvas inside the temple. 
The maze is designed as a puzzle. The user learns to collect items but is not sure why untiil they enter the inner temple. The items collected are a coin to open the main door, four items to collect a full date and a key to open the inner temple door. Entry into the inner temple leads to a canvas which is an invite to a celebratiion in the format of "Save the Date". There is a treasure chest. When opened the venue is displayed.
At this poiint a canvas is displayed to allow the user to restart the game.
Interactive UI canvases are used to iinform the user that the main door can't be opened without a oin and that a key and the full date items are needed to open the temple door.
Collection of items is rewarded with sound and animated particles.

* Audio
--------
* 3D spatial positioning audio placed on Canvas inside Temple - plays on awake at start of game - soundtrack barely audible at start of scene bu iincreases as user moves nearer to Temple Chest
* Audio setting set for gvr spatializer and using Oculus to set for 3D sound - logarithmic curve altered in 3D audio source settings positione on audio source on chest game object
* Other sounds such door opening, door closed, waypoints, collecting the key are placed via audio sources directly onto gameobjects and controlled by scripts - audio sounds set as public vars so can easily be changed
* 

