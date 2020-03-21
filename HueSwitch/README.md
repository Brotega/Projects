# HueSwitch

## Instructions to play HueSwitch
Download or clone the entire Projects folder if you haven't already. Navigate to the HueSwitch folder and go to either Windows 
or Mac folder, depending on the operating system you're using. If you're on a Windows PC, run HueSwitch.exe. Otherwise if you're 
on a Mac PC, run the HueSwitch.app. **If any problems are encountered contact me at ortegaam@usc.edu, and I will fix it as 
soon as possible.**

## Game Description
HueSwitch is a 2D puzzle platformer game that takes place in a 3D world. Most of the world has lost its color, and it is up to 
an angel to restore color back to the world. With the help of 4 colored spirits, the angel is able to rotate the world around 
him and access parts of the world it couldn't before. Use the spirits' power to navigate around and unlock all the doors that 
are hiding the stolen colors. 

HueSwitch is developed in Unity using the C# programming language. Developed between me and my 
design partner, with help from students at the Berklee College of Music. HueSwitch is available for Windows/Mac.

## My role
I did all of the gameplay/tools programming, small VFX, character art/rigging for this game. Here's the list of everything I implemented:
- Tools: Used 3D math to auto generate the colliders for all platforms, based on where the platforms are located in the world. 
Calculations are done at the very beginning of runtime. This made it easier for my level designer to place platforms without 
manually creating every collider in the Unity inspector
- Player controls: Standard movement, jump, rotating the character, previewing other sides of the world
- World events: Used raycasting off the camera to detect color of new background after rotating the world. Based on that new
background, every same-colored platform that is in front of that background gets deactivated. I used delegates to notify other 
classes whenever player would rotate the world.
- Key/Door interactions: Detect if player collides with key's trigger collider to pick it up. Player can grab keys and can only 
unlock certain doors if that door has the same matching key color. Implemented SFX, that was given to us by our sound team,
that plays whenever player picks up key or unlocks door. Used a "list" data structure to keep track of what keys the player has 
- UI: Programmed UI to keep track of what keys the player currently has
- End state: Created a level complete feature, where the camera breaks from the player and changes from orthographic projection to 
perspective projection. The camera would spiral down around the 3D world as we see color slightly restored to the world.
- Pause functionality: Pressing ESC that opens a pause menu, stops the game from updating, and lets the player select between 
"Resume," "Restart," "Main Menu," and "Quit" using their keyboard.
- Level select functionality: Created a system where player cannot advance to other levels without completing prior levels. There 
are three levels total. For each new level I added layered sound track given to us by the sound team.
- Spirits: Used Unity's particle system to create the spirits and programmed them to follow the player. The left and right spirits 
correspond to the colors of the background the player can switch into.
- Character: Used Clip Studio Paint to draw and create the angel character. By saving the as a .psb file, I rigged the character
using a Unity animation tool. Created idle, walking, jump, and falling animations. I programmed the character to use the 
appropriate animation based on their state.

## Trailer
Our game has a trailer you can check out! Here's the link: https://www.youtube.com/watch?v=1iYWJACtWKE

## Other
- This game will receive further development in the near future. The art and narrative are highly likely to change. Current 
gameplay elements will remain the same.
- As of January 15, 2020, this game has been submitted for the USC Games Expo 2020. Waiting for approval; hopefully it gets 
shown there!
