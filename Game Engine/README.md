# Game Engine
**In this folder are images of the engine. To see the engine in motion, look under the Video Link header and click on the link 
provided. The same video is also included in this folder if you downloaded/cloned the Projects folder.**

## Description
This is a game engine I worked on for a class project. The engine is written in C++11 using DirectX 11 and HLSL for Windows PC.

## Video Link
To see the engine, check it out here: https://youtu.be/eWf2pcLqX7U

## My role
Implemented many features of the game engine:
- JSON parser for creating the game scene. Parsed character, light, and object information (vertices) to later render in the graphics pipeline.  
- Graphics (real-time rendering): Initialization, processing vertex data from JSON parser to send to gpu, normal mapping, texture wrapping, skinning, lighting calculations (spotlight, ambient light), transforming position from local->world->projection space, transforming normals from local->world space, vertex/fragment shaders (phong with a few other variations of it, unlit).  
- 3D skeletal animation for character using matrix math
- Profiling for keeping track of performance
- Memory allocation for allocating static lights
- Physics: gravity simulation, AABB collision detection, raycasting
- Moving the player based on user input.
- Multithreading for calculating 3D animations on a different thread
