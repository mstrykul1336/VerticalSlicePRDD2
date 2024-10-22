# VerticalSlicePRDD2
 Vertical Slice PRD 2 of Shadows Over Suburbia
**Play:**
Play: https://mstrykul1336.github.io/VerticalSlicePRDD2/
**Link to Full Project:**
https://github.com/mstrykul1336/Shadows-Over-Suburbia-Prototype-
**Credits:**
First Person Controller: https://assetstore.unity.com/packages/3d/characters/modular-first-person-controller-189884?srsltid=AfmBOorWmRFs9bx7ebwFwd15ni4eQk7cPH1-OeGcAaLAW0HUaVO0Xw5H
ChatGPT for questions and bugs, learning how to do certain things I haven't done before in Unity.
Canva for demo asset icons (I will be drawing some of them later) 
Fantasy Forest Village: https://assetstore.unity.com/packages/3d/environments/fantasy/fantasy-forest-village-123484
Polygon City Pack: 
https://assetstore.unity.com/packages/3d/polygon-city-pack-environment-and-interior-free-101685
Farland Skies:
https://assetstore.unity.com/packages/2d/textures-materials/sky/farland-skies-cloudy-crown-60004
Fantasy Terrain Textures: 
https://assetstore.unity.com/packages/2d/textures-materials/free-fantasy-terrain-textures-233640
Fantasy Towns Music Pack: 
https://chrislsound.itch.io/fantasy-towns-music-pack

**10/21/24:**
**What was done:**
- Made the voting UI cleaner and better by adding a background image, adding an image to the button, and adding some text to explain it. 
- Added in font everywhere that matches the game’s aesthetic. (similar to Luigi’s Mansion)
- Added in the town scene at the title screen with lighting and effects. This will be used later for animations. 
- Added in a keyboard image with all controls into Controls in title screen
- Added theme music to the title screen. 
- Added in abilities for:
- Clairvoyant: Can check two players to see if they are friends or enemies with each other. (Will not reveal neutral role)
- Assistant: Can check the alignment of a player. (Will reveal neutral role)
- Detective: Can watch one player for a night to see what actions they take. (Even if they take the action before or after you investigate them)
- Old Man: Vote counts for two votes when they vote. 
- Villager: Can attack a player for 1/4th heart. 
- Added in new spawn points so players stopped spawning on top of each other. 
- Added in text UI for when you are attacked or healed, just so you know why your hearts randomly go up or drop. (this currently isn’t working, not sure why the RPC calls are being messed up)
- Added new UI for each ability to differentiate them. 
- Added in functionality for the shield, so if it is used at night, it will block any attacks (currently poison or other damage). It will not block you from being poisoned though, just from not being damaged for one instance. 
- Items will be removed from inventory after use. 
- Poison damage and villager damage are still a bit buggy, usually it will attack you for twice the amount with poison damage on the first day it happens. Sometimes it will correctly attack you for the right amount. 
- Added in randomized death image newspapers for when players die to make it more fun. Player’s name that died will appear in the newspaper. There are around 7 different newspapers to get!
- Player UI List thing is still messed up, spacing is weird. 
- Knife is still buggy, but it might work. Made sure it leaves the inventory when done with and that it has everything in place to work. 
- Changed the player and party room texts to fit the theme of the game. 
- Added in the 1 button to toggle player movement on and off. 

Backlog for next week: 
Changing players from disconnecting to spectating as ghosts (make sure in every loop that calls playerList that it also checks to make sure they aren’t dead.)
Add in their roles into the newspaper if they die too (and eventually their profile picture image)

**To Do:**
Add in abilities for the rest of the roles that get them:  
Detective: Investigation (watch one player at night to see what happens to them) 
Assistant: Connections (discover if a target player attacks anyone tonight) 
Clairvoyant: Psychic (can select two players to learn if they are friendly or enemies to each other, based on helpful or destructive) 
Old man: Voter Fraud (can vote twice instead of once) 
Villagers: Attack (can attack people for ¼ heart) 
Add in UI for attacks so you know that you were attacked or taken or healed, whatever happened to you. 
Make the shield work as intended and actually block an attack at night (it should block poison, bleed, and normal attacks) 
Bug check the knife to make sure it properly attacks players, attacks player in the dropdown provided.  
I believe it does, but make sure the inventory actually takes the item out when it is used.  
Make a cool UI (image or video, but WEBGL hates videos) for when players die (randomly show different versions of the UI of them dying, like minecraft changes the text). Maybe change this to animation loaded elsewhere with the player’s model and a random death scene.  
Make the voting UI better and cleaner.  
Clean up the player list UI.  
Add in a font that matches the aesthetic for all text in the game.

**Backlog:**
Add in destructive and helpful versions of these abilities:   
Mayor: (currently has mayor's basement for helpful, but if destructive, you will be able to sacrifice the player to WiggleBlorp) 
Assistant (destructive would get brainwash, where you send an anonymous message to a player to invite them to the cult (destructive) side).  
Detective (destructive would get unlawful investigation, same investigation but you get the option to attack them, causing them to bleed for 1/4 hearts DOT for 3 nights) 
Medic (currently has heal, would need fake heal for destructive where it makes another player believe they were attacked and then healed) 
Everyone else gets the same ability no matter what side. 
Add in passives to two characters: Medic (immune to poison and bleed) & Clairvoyant (can't die at night, needs to be voted out). I need to make it so it doesn't give away their characters to any players though, just doesn't end up working if you attack them. 
- I want to try to make it so instead of disconnecting players, they can spectate as ghosts, but can't interact. I think this should work out as long as in all my loops that go through player list, I also check if the player is not dead before adding them to whatever.
- And add in that button to toggle player movement or not.

