# 3DMaze

A recreation of the classic 3D Maze screensaver that was present in Microsoft Windows 95 using Unity.

## Overview

The maze is randomly generated each time, with the "player" navigating through it in first-person, spawning in front of a floating start button. From there, the maze is automatically traversed using the left-hand rule, which will guarantee the maze will eventually be solved because all of the randomly-generated mazes are simply connected.

By default, the maze is textured with brick walls, a wooden floor, and an asbestos tile ceiling. Users can customize these textures, swapping them out for animated psychedelic patterns in later versions, or may instead create their own custom textures.

As the maze is traversed, several objects can be found inside it, including floating "OpenGL" logos, images of globes on the walls (which is seen on the cover of the OpenGL Programming Guide), and a 2D sprite image of a rat that is also moving through the maze. Additionally, the "player" will encounter rotating polyhedric gray rocks that, when touched, will flip the camera upside down and turn the floor into the ceiling. When this happens, the "player" will traverse the maze following the right wall rather than the left until the exit is found or another gray rock is encountered.

The exit to the maze is a floating, translucent smiley face. Upon reaching it, the maze will reset and another will be generated.

Users can also enable an overlaid map, which constantly displays the maze using simple vector graphics. On this map, the "player" is represented as a blue triangle, the start as a red triangle, the smiley face as a green triangle, the rocks as rotating white triangles, the OpenGL logos as stationary white triangles, and the rat as an orange triangle.

## Keyboard Commands

* WASD to walk left, right, up, down
* Left Shift or Right Mouse Button to run

## Project Information

The project uses standard Unity files and assets. Nothing special needed here. 

The Player Input setup uses the default so movement is controlled via the Horizontal and Vertical inputs with the Run key bound to Fire3 (which by default is Left Shift or the Right Mouse Button).

There is no UI or menu. There's only one scene in the build. Pressing ESC will exit the game (if running the executable) or stop playing in the editor. 

Player control, by default, is set to the original control. This allows you to travel the maze in a grid like fashion (like the old Eye of the Beholder games) moving square by square. The modern control option is a free roam with mouse control. This is set by the Control Type dropdown on the Player object in the scene.

## History

3D Maze is the name given to a screensaver, created in OpenGL, that was present in Microsoft Windows from Windows 95[1] until it was discontinued after Windows ME.

## Requirements

* Unity 2021.x or higher (not tested with Unity 2022.x, might work on versions earlier than 2021 too)
