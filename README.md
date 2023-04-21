---
description: 'SCP: Containment Breach Map Creator Version 2.1 Manual'
---

# English

## Startup

After starting the map creator, you can either create an entirely new map or load an existing map and edit it.

If you opened the map creator for the first time you might need to navigate to the map folder on your own to select the maps. However, the path should then be saved after the first use.

If you save a map you also have to make sure the saving path is the one where the map files are stored (`Map Creator/Maps`). This is important as the original game checks this path to find maps that can be loaded.

## How to build a map

Before creating a map it is important that you know the basics of how to create a map for SCP - Containment Breach.

At the very left of the program, there is a list of rooms that can be placed on the map grid. A short description of the room will appear below the list, as well as a selection box that contains events that can be selected for the room (if any).

A short description of the event will appear below the event selection box. The probability of the event appearing in the room can be modified by the slider below the event description.

* The percentage means how likely it is for the event to happen. `100%` is the default value and means the event always occurs.
* In order to prevent a certain room from having events you can select **\[none]** in the event selection box.

Below the event probability slider is yet another text box that is used to show the stats of the selected room.

The grid at the right side of the window is used to place the rooms on the map. Rooms are placed simply by selecting one from the list and then clicking on the square you want to place it on. You can select placed rooms by clicking on them. You can rotate the selected room by holding the left mouse button. The rotation can be seen at the bottom left corner where the room stats are displayed.

### Note

* By selecting a room on the grid you deselect the entry from the room list. You need to double-click on the same room name in order to select it. If a plus appears when you move the mouse over the grid it means you can place a room on a square.
* The "start" room (SCP-173's containment chamber after the intro sequence) always has the rotation set to 180 degrees and it can't be changed. This is due to the scripted sequences at the start of the game which require the room to be oriented in a specific way.
* The checkpoint rooms have the rotation set to 180 degrees so they automatically face the correct directions. However, their rotation can be modified, unlike that of the "start" room.
* The "start" room (SCP-173's chamber) and the "alarm" event are required for the game to work correctly.
* The option "**Set the Event for the rooms by Default**" determines if a room should get an event assigned automatically upon placing it on the grid (usually the first one that appears in the event's selection box).
* The option "Place adjacent doors in 3d view" determines if the doors leading to another room should be displayed in the 3d viewer or not. This is useful for determining which zone a room is located in.
* The option "**Map Settings**" allows you to modify the borders between each zone. Click on "**Apply**" to apply the changes and click on "Reset" to reset the borders to the default settings.
* You can edit the author name and description of the map by clicking the option "**Edit Author and Description**". The setting is automatically saved when you close the window.
* There are three different types of grids you can modify: The Facility, the Forest, and the Maintenance Tunnels. The Facility grid is the default grid used to place all the rooms and events. The forest grid is used for SCP-860-1. Note that you need to place a "room860" with its event set to a chance of 100% to make this grid appear. The same applies to the Maintenance Tunnels, except that it requires the event "room2tunnel". Note that whenever you change the grid, the list of rooms changes as well. The SCP-860-1 and Maintenance Tunnels grids are viewable in the 3d viewer as well.

You can delete a room by right-clicking the room icon on the grid. By holding the right mouse button and swiping over the grid you can delete multiple rooms at once.

Clicking the middle mouse button deselects the currently selected room.

You can also search for certain rooms by typing something into the search box that is above the room's list box and clicking on the "Search" button. The search box can be cleared by clicking the "**X**" button next to it.

**Important:** Whenever you save a map you are given the option to save it as a "`cbmap`" or "`cbmap2`" file. "`cbmap`" is an outdated format (although still compatible) and "`cbmap2`" is the new one that is able to save the author's name, description, zone transitions, and the forest and maintenance tunnel grids.

## 3D viewer options

This version of the map creator also has a 3D viewer. It can be accessed by clicking on the "**3D/Map Viewer**" button at the top left-hand corner right next to the "**2D/Map Creator**" button. The "**2D/Map Creator**" button will bring you back to the 2D view of the map creator.

The options for the 3D viewer are located at "**Options** -> **Edit Camera**":

* **Change CameraFog Color**: This option changes the background color of the 3d viewer. The default color is black (R=0, G=0, B=0).
* **Change Cursor Color**: Changes the color of the cursor that can be seen when entering the free-flight mode of the 3d viewer. The default color is red (R=255, G=0, B=0).
* **Culling Range**: Determines the range on how far away from the camera a room should still be rendered. The default value is `50`. Note that the further the culling range is, the more rooms will render at once. A too-large value may cause performance issues.
* **VSync**: Determines if the rendering rate should be synced with your monitor's refresh rate.
* **Show FPS**: Determines if the framerate will be displayed in free-flight mode.

## 3D viewer controls

When you have selected a room by clicking it on the grid and going to the 3d viewer, the camera will focus on that room. If you do not wish for the camera to move, deselect any rooms before switching to the 3D viewer.

You can enter the free-flight mode by right-clicking on the 3D viewer window. Use the W/A/S/D keys and the mouse to move the camera around. Rooms can be highlighted by moving the cursor over them in free-flight mode. Additionally, you can see the name, the X and Z coordinates, and the event assigned to the room.

By left-clicking on a highlighted room you select it in the 2d grid as well, allowing you to easily modify a room on the grid if necessary.
