WhaleGame

Player Mechanics

WHALE:
Movement: Momentum based, with player input required to move tail to generate thrust/momentum. These inputs can have an effect on O2 depletion/hunger build up. Spamming inputs can produce a quick burst of speed but with decaying efficiency and ramping O2 consumption. Conserve O2 on ascents/descents into the depths by letting the relative density of the water pull the whale up/down.
Movement can be increased by increasing whale size.
Movement can be impeded by being harpooned, or trapped in fishing nets.
Low health will also impede movement.

Player position will remain locked to the center of the screen, such that the player doesn’t really move, instead the world moves around them. Game will have to keep track of player’s position relative to the water’s surface in order to inform breath mechanic as well as depth/pressure mechanic, and light..

Echolocation: Whale can generate loud clicks in order “see” at depths where light is scarce. Clicks will travel out from the player as a projectile (or cone?), and on collision with an object will then highlight the edges of that object against the dark world background, “illuminating” the object within the scene.
Holding down the button for echolocation can charge a “louder” click which will temporarily zoom the camera out and emit a large cone in front of the player illuminating distant objects.
Spamming the echolocation button in short succession will limit the range of the click projectiles, but can be used to stun prey, inhibiting their movement.
For objects capable of movement, “illumination” will only reveal the position at the time of click collision. Click collision will create a clone of the object that is non-interactable.
“Illumination” on objects will slowly fade out over a brief period of time.

Meter Management:
Health: HP begins to deplete when other resources are depleted, or upon taking damage from various sources.
Health will regen slowly over time if Hunger is not too high.
Once health drops below a threshold (50%, 40%, 30%?), scaling negative effects begin to set in; reduction in movement speed, lung capacity, slowed rate of healing

O2: Depletes as long as player is below the water’s surface. 
Depletion rate increases with continuous/prolonged movement. Reduce overall movement by taking advantage of relative density to descend.
Max O2 limited by HP falling below threshold.

Hunger: Slowly rises at a continuous rate. Can be held back by consumption of prey (fish, squid, giant squid)
As whale size increases hunger rate also increases, requiring larger amounts of food to fuel metabolism.
Remaining satiated will increase rate of healing, and provide small buff to movement speed.

Whale Size: Consistent maintenance of Hunger/HP will precipitate growth over time. A larger whale requires more food to remain satiated and will make a whale a bigger target for whalers. However size can confer some advantages such as being able to:
move faster/further, 
increased lung capacity, 
increased depth tolerance, 
increased echolocation range, 
and the ability to capsize small boats, 
or more easily break free from nets.


Non-Player Mechanics
ECOSYSTEM
Fish: Governed by Boids flocking behavior, serves as food source for player early in the game, but ultimately not favored food.

Squid: Prey on fish, a favored food source with offering more hunger satiation. Squid have more erratic movement when compared to fish.
Can eject ink in order to inhibit player vision, however usage of echolocation will mitigate the impediment this presents.

Giant Squid: Highest value food source, however is more difficult to find, generally only appearing at significant depth, and has the capability of harming the player.

HUMANS
Fishermen: attracted to congregating fish. Source of competition for player over food. Multiple variants: small and large; using nets of varying size. Nets can impede player movement.
Nets: Player collision with a net will initiate a struggle event where the player has to spam movement inputs in order to break free. The threshold for breaking free will be random but will scale with the size of the net/size of the player.

Whalers: use harpoons to attempt to spear player. Can cause bleeds on the player leading to damage to health over time. Harpoons with rope, will tether the player to the whaler’s vessel, forcing the player to drag the vessel. This will impede movement, slowing movement speed, and preventing diving unless sufficient speed is built up to dislodge the harpoon. Player can flip/capsize smaller whaler vessels dependent on player size. Breaching the surface will potentially attract whalers to the player’s last known surface position.

