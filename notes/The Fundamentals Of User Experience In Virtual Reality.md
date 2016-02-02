#### Notes from thejourneydude:

- biggest considerations when switching from desktop games to vr games
    - comfort: one of the biggest pet peeves
        - if you don’t have comfort settings in your menu settings, then users will dislike it

        - every user is different: some get motion sickness while others do not

        - setting options such as blink mode which eliminates the animation when moving from one point to another in small steps

        - Alternate control schemes, supporting as many input devices as possible, and doing lots and lots of testing will be just some of the ways you can make your players experience more comfortable.

        - for smash hit plunder they first run a quick test determining how motion sickness someone can become by having the user move at a constant acceleration in steps.

        - the user can then adjust different settings:
            - 1) blink mode: described above

            - 2) dark mode: while moving the users vision becomes black, where they only see their feet moving, a way to know that they are at least moving

            - 3) normal mode: the user points at a location they want to go to, a marker is placed at that location and at a constant acceleration the player moves to that marker. because the marker exists the user feels like the world is moving, not them. if the marker is removed the user may wobble backwards.
        - most people think blink mode is most comfortable.
    - interface:
        - we can no longer snap interfaces to the player’s face like we did in traditional games

        - interfaces now need to exist within the game world or mounted to some kind of external zone rather than the head.

        - buttons and menus will also need to change to accommodate field of view

        - because of the current vR headset have low resolution, text and buttons also need to be larger and more distinguishable
    - sound and music:
        - its important to not just slap audio into your app/game, you will need to make sure the sound is immersive as well as be positional
    - movement:
        - WASD may die because of VR

        - there are no more simulated barriers between the user and the environment(like a computer screen)

        - the approach to movement will depend entirely on you

        - making a simulated body doesn’t feel as immersive. games with some kind of ship or care work really well in VR because the environment is moving around the vehicle, whereas making a simulated body doesn’t feel as immersive.

        - take standing vs. sitting into account.
    - interaction
        - vr may spell the end of the mouse cursor and click for interacting with elements

        - a lot of interactions are being played around with and tested, and most are shown to be largely devise dependent
    - normal maps:
        - normal maps don’t work well in VR in a lot of cases

        - this is because the eye is very good at picking out depth information - because VR is stereoscopic by default - we see normal maps as flat or lacking all of the depth information to signify this object has depth.

        - what all of this means is that geometry has to carry the weight of immersion much more than normal maps

        - its a good idea to only use normal maps on objects that will be far away from the player since the
        parallax effect will be negligible beyond a certain distance.

        - this doesn’t mean you use normal maps, but if you try to use normal maps to convey depth on objects that are near the player, you’re going to fight against immersion.
    - model detail:
        - close objects need to be finely detailed.

        - you can cut costs on far away objects, but not nearby ones
    - user testing:
        - will be more critical than ever before

        - need to ensure no one gets sick, designed environments make sense from a 3D spacial standpoint

        - questions like:
                - can users figure out where to go

                - Are there visual or spacial audio cues about what to do next or where to look?
