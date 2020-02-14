# forReview

Ikecode is called on server poll.  It is the engine that calls  the other routines.  It has the routines for social mob behavior, mob migration, custom spells etc.  Mob migration does mobs in incremental bites each poll and monitors the duration of the work.  If the duration exceeds a certain amount of time, it reduces the size of the bites each poll until the duration is within an acceptable range.  

Guardian is the combat pet code. The combat pets use existing skills that don't apply to pets to hold information.  So skill #1013 (I don't remember what that is) holds the last command issued by the player via his wand).

WispUpdate is the light token that follows the player around.

Fireorb spell just applies an initial damage and a spell effect.  Ikecode CustomSpellsUpdate handles the dot effect.

IronFloor is just strongwall for cave floors

Spark spell does initial damage and applies a spell effect.  Spread of spark to other mobs is handled in Ikecode CustomspellsUpdate



