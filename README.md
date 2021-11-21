# HA1
3d platformer with procedural level generation
## Design document
### Name
HA1
### Description
Third person 3d platformer with endless number of levels and increasing difficulty
### Main character
Regular third person character
### Plot
There is no plot for ha1
### Gameplay
#### Goal
The goal is to reach the highest level
#### Game mechanics
* Player can run on platforms
* Player can jump
* Player dies when falls or collides with deadly objects
* After death player starts from the beginning of the current level
* Player can be knocked off by moving/spinning objects on the platform
* Player can collect coins to buy boost
* Player can walk through walls when boost is activated
* Moving/spinning platforms and objects on them become faster every level
* Player can buy boost if there are enough coins
* Boost lasts for 30 seconds
* Only one boost can be used at a time
* Only one boost can be used at each level
* Player can collect coins
### Graphics and styling
* The game has colorful square and round platforms
* Some platforms have walls, spikes or cubes on them
* Glowing red color indicates deadly objects
* During the game player can see the current level, number of collected coins and the timer for activated boost
### Music and sounds
The game does not have any sound
### Technologies
The game was developed using Unreal Engine 4.27 for Windows 10 or higher
## Description of level generation and increasing complexity
### Level generation
Number of platforms depends on the level, formula is following: max(5, 2 * level).  
Choice of platforms is random, only first and last platforms are specific.  
There are 2 boosts on the first platform for the player to choose.
### Increasing complexity
Platforms and objects on them move/spin faster every round. At the first few levels some platforms are not available.
## Description of bonuses
### Coins
There are coins that player collects. These coins are randomly spawned on some platforms.
### Boosts
There are 2 boosts in the game that player can buy for 5 coins:
* Passing through walls but deadly walls still kill the player
* Slowdown mode which slows every moving/spinning platform or object by 3  
Boost can be activated at the beginning of the level\
Only one boost can be activated at a time
## Description of moving obstacles
### Moving platform
There are 3 types of moving platforms:
* Platforms that move along the Y or Z axis
  * Platforms become moving with 50% probability 
  * Axis is chosen randomly
* Falling platforms
  * This platform starts falling when player steps on it and go back to their place once there is no player on it
  * Platform falls so far that player dies
 * Spinning platforms
### Moving obstacles
* Spinning wall
* Spinning deadly wall collision with which is fatal
* Wall that reaches player when he steps on the platform
* Moving deadly cube that moves in a zigzag manner, collision with this cube is also fatal
## Assets
All assets (spikes, crystal, coin) are taken from https://sketchfab.com/
