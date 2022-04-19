# STEAM Engineers workshop

## Introduction
Today we're going to look at making video games with Makecode. Once your game is finished you can play it here or share it to see who gets the high score

## Introduction
The part of the screen that looks like squared paper is where our code will go. 
All the code blocks are in the next column. They are grouped by the type of thing they do

## Let's get started.

Ready to write your code? From the ``||game:Game||`` menu click and drag a ``||game:splash("")||`` block and connect it to the ``||loops:on start||`` block that is already there.

## Splash
The block we have just added will be what we see before the game starts. Type a messgage into the white bubble. Whoever is playing your game will see this until they press button A.
Test it works in the simulator

## Set the scene
Now we are going to set the background for our game. It's going to be set underwater, so it should probably be blue.
From ``||scene:Scene||`` grab a ``||scene:set background color to()||`` and join it to your code.
Click on the grey rectangle to set the colour

## Add some effects
Drag the ``||scene:start screen [confetti] effect ⊕||`` from the  ``||scene:Scene||`` category and
into the ``||loops:on start||`` block. Change the effect to ``||scene:bubbles||``

## Draw your own background
The last block for the background is ``||scene:Set Background Image to ⊕||`` from the  ``||scene:Scene||`` category.
Clicking on the rectangle will open the image editor. Get creative and make some seaweed for your game.

## Adding a player
In video games anything that moves is called a ``||Sprite||``
Grab a ``||variables:set [mySprite] to sprite [ ] of kind [Player]||`` from the ``||sprites:Sprites||`` category.
Add this to the bottom of your code

## Drawing our character
Click on the grey box in the middle of your  ``||variables:set [mySprite] to sprite [ ] of kind [Player]||`` block
to open the image editor.
Either draw your own fish, or choose one from the gallery.

## Making it move
Great so we have our player, now to make it move.
In the ``||controller:Controller||`` category get a ``||controller:Move my sprite with buttons()||`` block and add it to the end of your code
Test this code and make sure your fish can swim!

## Adding enemies
To add enemies we're going to use a new type of block. From ``||game:Game||`` get a ``||game:On game update every 500 ms||`` block.
This looks slightly different to the other blocks. It can't click onto the bottom of
our code, put it alongside our start block.

## On game update
The onstart block code runs once when we start the game. Our new block, ``||game:On game update every 500 ms||``, runs every 500ms (half a second).
So we can use it to make lots of enemies!

## Add enemy sprite
In the ``||sprites:Sprites||`` category scroll down to find the projectiles section.
Grab a ``||sprites:Set Projectile to projectile from side with....||`` block and add it to ``||game:On game update every 500 ms||``

##Draw the shark
Our enemies are going to be sharks, click on the grey box to open the image editor.
Draw your enemy shark, or pick one from the gallery.

## vx and vy
You might have noticed, at the end of the block are numbers labelled vx and vy.
These tell us how fast our enemies can move. 
Change vy to 0, so the enemies can move sideways but not up and down.

## Add randomness
At the moment all our enemies swim in a line, that makes them reall easy to avoid.
From ``||sprites:Sprites||`` get a ``||sprites:Set my sprite x to 0||`` block, add this to our new code.

## Set randomness
In the ``||sprites:Set my sprite x to 0||`` block change ``||sprites:mySprite||`` to ``||sprites:projectile||``
Also change x to y using the dopdown menu.

## Set randomness
From the ``||math:Math||`` get a ``||math:Pick random 0 to 10||`` and plug it into the white circle in our ``||sprites:Set my sprite x to 0||`` block.
Change the numbers to 10 and 110

## When the enemy catches us
So we have a player we can move around, and things for them to catch. The last step is to tell the game what to do when we collect them.
From ``||sprites:Sprites||`` find the Overlaps section and get a ``||sprites:On Sprite of kind player overlaps with...||``
Place this next to your other code.

## Overlaps
This new code block runs everytime our player touches an enemy sprite.
After ‘other sprite’ use the dropdown menu to change player to projectile.
What should happen when our player hits an enemy?

## Info

In the ``||info:Info||`` category is ``||info:Life||`` Grab a ``||info:Change life by -1||``
You will also need to add a block to the ``||loops:on start||`` to set the number of lives we start with.

## Music
Can you work out how to add a sound that plays if we hit an enemy?

## Rewards
Using what we've learned so far can you work out how to add another type of projectile that we have to collect to earn points?
