# Sword-of-Mana-Mods
Fixes and Mods for Sword of Mana


**som_perf_plus2_pathing.bps**

This patch adds 30%+ performance patch that stops most slowdowns to keep the game at 60fps, it uses some extra iwram along with some changes to the way sprites are drawn in return for better frame rates. It has some failsafe check built in so crashes are unlikely, I have not encountered any crashes yet and the FPS remains close to 60FPS in most areas with heavy sprites on screen. Further improvement is possible but so far this seems adequate.

This patch also add pathfinding to the NPC courtesy of Gentlefox for his work on enemy pathfinding in Shining Souls 2. The NPC will now navigate around obstacles and walls much much better. It can still become stuck when enemies are directly blocking them but its very rare. 

I also added some behavior changes to the NPC. I increased the run speed so the npc will keep up with you and eliminated the "Wander" code in the NPC behavior since it is no longer needed for navigation. I changed the leash code to keep it closer to your character to prevent them from getting stuck and lost. I added 2 sliders you can modify 

1. Chase Slider = Changes the enemy chase range. Useful for range NPCs so they don't endlessly get stuck casting spells while your running away.
2. Distance Slider = How far the NPC stands from you. For range NPCs, it keeps them from enemy melee range when you are attacking. For Melee NPCs it'll keep them closer to you to act more like tanks/bodyguards


**som_pathing.bps**

This patch is only the NPC pathfinding and behavior/slider changes and does not include the Performance enhancements in case a a bug is found that causes crashes.
