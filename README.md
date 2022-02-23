# STEAM Engineers workshop

## Introduction
Today we're going to look at making video games with Makecode. Once your game is finished you can play it here or share it to see who gets the high score

## Introduction
The part of the screen that looks like squared paper is where our code will go. 
All the code blocks are in the next column. They are grouped by the type of thing they do

## Let's get started.

Ready to write your code? From the ``||game:Game||`` menu click and drag a ``||game:splash("")||`` block and connect it to the ``||loops:on start||`` block that is already there.
If you are not sure, click on the lightbulb for a hint.
```blocks

game.splash()

```

## Splash
The block we have just added will be what we see before the game starts. Type a messgage into the white bubble. Whoever is playing your game will see this until they press button A.
Test it works in the simulator

## Set the scene
Now we are going to set the background for our game. It's going to be set underwater, so it should probably be blue.
From ``||scene:Scene||`` grab a ``||scene:set background color to()||`` and join it to your code.
Click on the grey rectangle to set the colour
```blocks

game.splash()
scene.setBackgroundColor()
```
## Add some effects
Drag the ``||scene:start screen [confetti] effect ⊕||`` from the  ``||scene:Scene||`` category and
into the ``||loops:on start||`` block. Change the effect to ``||scene:bubbles||``
```blocks

game.splash()
scene.setBackgroundColor()
// @highlight
effects.bubbles.startScreenEffect()
```
## Draw your own background
The last block for the background is ``||scene:Set Background Image to ⊕||`` from the  ``||scene:Scene||`` category.
Clicking on the rectangle will open the image editor. Get creative and make some seaweed for your game.

```blocks

game.splash()
scene.setBackgroundColor()
effects.bubbles.startScreenEffect()
// @highlight
scene.setBackgroundImage()
```

## Adding a player
In video games anything that moves is called a ``||Sprite||``
Grab a ``||variables:set [mySprite] to sprite [ ] of kind [Player]||`` from the ``||sprites:Sprites||`` category.
Add this to the bottom of your code


## Drawing our character
Click on the grey box in the middle of your  ``||variables:set [mySprite] to sprite [ ] of kind [Player]||`` block
to open the image editor.
Either draw your own fish, or choose one from the gallery.
