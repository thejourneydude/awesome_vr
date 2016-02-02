#### Notes from thejourneydude:

##### Part 1. User Interface Design

- The “physical” design of interactive elements in VR should afford particular uses.

- Every interactive object should respond to any casual movement.

- Clearly describe necessary gestures with text-based prompts.

- Interactive elements should be appropriately scaled.

-  Place text and images on slightly curved concave surfaces

- When an interaction relies on a user moving in a certain way, or making a specific pose, create affordances to encourage this.

- The most 2 reliable “intuitive gestures” are ones where we guide users into doing the proper gesture through affordance.

- By thinking about how we understand real-world objects, you can harness the power of hands for digital experiences

- there are two type of gestures
    - semantic: based on ideas about the world. vary widely from person to person

    - responsive: occur in response to the ergonomics and affordances of specific objects. They are grounded and specific, making them easy to track. Because there is a limited range of specific interactions, multiple users will perform the exact same gestures.

- affordance: refers to the physical characteristics of an object that guide the user in using that object. well-designed affordances on a physical object encourage correct use and prevent incorrect use.

- best practices for designing interfaces in VR:
    - the more physical the response of an object, the wider the range of interactions may be correctly responded to. for example, a physical piston acting like a button needs to look pushable.

    - the more specific the interaction, the more specific the affordance should appear. in other words, the right affordance can only be used in one way

    - Look for real-world affordances that you can reflect in your own projects.
- Every interactive object should respond to any casual movement.

- its important to use certain cues to show a user they interacted with an object. below are some points when handling a button
    - use a shadow from the hand to indicate where the user’s hand is in relation to button

    - create a glow from the button that can be reflected on the hand to help understand the depth relationship

    - ensure the button moves in relationship to the amount of pressure (Z-press) from the user

    - use sound to indicate when the button has been pressed (“click”)

    - create a specific hover state and behavior for interaction widgets

- if an object appears intangible, people have no mental model for it, and will not be as able to reliably interact with it.

- text/audio based tutorial prompts can also help for first-time users. be sure to fully describe intended interactions.

- be descriptive as possible in your text description on how the user makes interactions

- interactive elements should be scaled to appropriate to the expected interaction.

- limit unintended interactions. space out your UI elements. or if depending on the nature of the interaction, have the first object of a group to be touched momentarily lock out all others

- limit hand interactivity. make a single element of the hand able to interact with buttons and other ui elements - typically the tip of the index finger. conversely, other nearby elements within the scene should not be interactive.

- because of current tech, rendering text is difficult. due to resolution limitations, only text at the center of your FOV may appear clear while text in the periphery may seem blurry unless users turn to view it directly.

- limit the angular range of text to be close to the center of the user’s field of view (e.g. making text appear on a surface only when a user is looking directly at the surface).

##### Part 2. Interaction Design

- no movement should take place unless it’s user-driven.

- keep in mind that human hands naturally move in arc, rather than straight lines

- limit the number of gestures that users are required to learn

- all interactions should have a distinct initiation and completion state

- ensure that users can interact with objects occluded by their hands

- being able to control movement reduces the experience of motion sickness

- the display should respond to the user’s movements at all time, without exception. even in menus, when the game is paused, or during cutscenes, users should be able to look around

- Do not instigate any movement without user input (including changing head orientation, translation of view, or field of view).

- do not rotate or move the horizon line or other large components of the environment unless it corresponds with the user’s real-world motions

- reduce neck strain with experiences that reward (but don’t require) a significant degree of looking around. try to restrict movement in the periphery

- ensure that the virtual camera rotate and move in a manner consistent with head and body movements

- when making a hand movement in Z, the user inherently makes a Y movement as well. the same is true when the user moves along the X axis - this motion will result in the user also creating a z movement.

- hand movements can also vary greatly based on posture.
    - pivoting on a fixed shoulder with elbow raised: wandering in the X and Y axes.

    - pivoting on a fixed elbow on a table: wandering in Y

    - movement pivoting on wrist with relaxing index: minimum wandering, very small Z depth

- There are a very limited number of gestures that users can remember.  most studies put this number at 5. When developing for 9 motion controls, be sure to build on a base set, or try combining gestures for more advanced features. Even better, create specific affordances that users will respond to, rather than having to learn a specific pose or movement.

- all interactions should have a distinct initiation and completion state. the more ambiguous the start and stop, the more like users will do it incorrectly
    - clearly describe intended poses and where the user should hold their hand to do that pose

    - if the intended interaction is a motion, make a clear indicator where the user can start and stop the motion

    - if the interaction is in response to an object, make it clear from the size and shape of the object how to start and stop the interaction

- people routinely interact with objects that are obscured by their hands.

- because users don’t have feedback to touch, we need to find alternative means for the user to know they are interacting with an object
    - provide audio cues to indicate when an interaction is taking place

    - make the user’s hand semi-transparent when near ui elements

    - make objects large enough to be seen around the user’s hand and fingers.

    - avoid placing objects too high in the scene, as this forces users to raise their hands up and block their view.

    - when designing hand interactions, consider the user’s perspective by looking at your hands with a VR headset

- Generally, the best VR applications that use Leap Motion for navigation aren’t centered around users “walking” around in a non-physical way, but transitioning between different states. Here are some interesting experiments in locomotion.
    - World of Comenius: users glowing orbs that can be tapped to travel from place to place

    - Fragmental: navigation controls let you revolve around a central axis. in other words, allows user to rotate around a central point

    - VR Intro: uses two handed flight to allow user to navigate. the problem is that it become a bit tiring unless its used shortly, or alongside other interactive elements

    - Planetarium: contains a ball that the user can use to move with small displacements from a  comfortable posture, while also providing compass data that helps to orient the user. the ball move slightly when the user is moving on

    - Three.js Camera Controls: shows different ways that users can navigate 3d space

- sound is essential aspect of immersive VR. also be  very effective in communicating the success or failure of interactions. it can be used to create the “illusion” of tactile sensation

- tactile sensation: button clicks on touchscreen keyboards help users become confident treating the keys as independent interactive objects. In particular, this provides useful feedback on interactions in the periphery of the user’s FOV.

##### Part 3. Optimizing for VR Tracking

- Include safe poses to avoid “the Midas touch” where everything is interactive.

- Encourage users to keep their fingers splayed out.

- Keep interactive elements in the “Goldilocks zone” between desk height and eye level.

- Filter out implausible hands.

- Use visual feedback to encourage users to keep their hands within the tracking zone.

- Avoid interactions involving fingers that would be invisible to the controller.

- demo must have a safe pose, so that users can 13 safely move through the device’s field of view without interacting.

- Gesture-based interactions should be initiated with specific gestures that are rarely a part of casual movement

- Do not require a pause to begin an interaction, as your users will become frustrated. an interaction should be tracked immediately.

- Whenever possible, encourage users to keep their fingers splayed and hands perpendicular to the field of view. This is the most reliable tracking pose.

- You can encourage this position by requiring interactions to be initiated from this pose, and provide positive indicators when the pose is detected

- Interactive elements should generally rest in the “Goldilocks zone.” This zone is between desk height and eye level.

- Allow a maximum of one right and one left hand, and only animate those two hands when tracking hand movements

- If the user can’t see their hand, they can’t use it. in essence, users much have their hands in view at all times

- here are some ways to ensure the user keeps their hands in view at all times
    - disappearing skins: when the hand is in view and is covered with a skin asset and the hand trackers has full confidence, then the skin is in full opacity. however, as the confidence drops, then the skin loses its opacity.

    - error zone: Delineate a clear safety zone to indicate where the hands should be placed. You can notify the user when their hands enter (or exit) the zone with a simple change in color or opacity to that area of the screen.

    - if the user picks something up with their hand, then it should be held by their hand until they release it. if the hand leaves the view while the object is still being held, gracefully handle the exit animation

    - there is the chance that hand gestures may either fail or exit the field of view. Your application should handle these in a way that yields smooth and plausible motion, without causing unintended interactions.

- be sure to avoid interactions that depend on the position of fingers when they are out of the device’s line of sight. For example, if pinching is allowed, it should only be possible when the fingers can be clearly seen by the controller. Similarly, grabbing is tracked most reliably when the palm faces away from the device.

##### Part 4. Hands and Body

- Create or select virtual hands that are appropriate to the setting.

- Virtual hand positions should match real-world positions as closely as possible.

- Only render the user’s body in situations where you can expect reasonable agreement. While being disembodied is disconcerting, having multiple inconsistent bodies is usually worse.

- hand positions must match their virtual counterparts as much as possible

- By providing a bodily relationship to the elements in the scene, you can increase immersion and help ground your user.

- people are generally comfortable if they have no body in vr. this is due to other similar experiences such as watching movies or the day to day interactions with the real world. if you do have a virtual body for the user, then ensure that the body matches the real-worlds body movement and position.

##### Part 5. Space and Perspective

- Adjust the scale of the hands to match your game environment.

- Align the real-world and virtual cameras for the best user experience.

- Use 3D cinematic tricks to create and reinforce a sense of depth.

- Objects rendered closer than 75 cm (within reach) may cause discomfort to some users due to the disparity between monocular lens focus and binocular aim.

- Use the appropriate frame of reference for virtual objects and UI elements.

- Use parallax, lighting, texture, and other cues to communicate depth and space.

- adjust scale of hand according to device in unity, unreal, etc.

- recommend to use 1:1 scale to make virtual hands and objects look as realistic and natural as possible

- for AR, the scale needs to be adjusted to match the images from the controller to human eyes. appropriate scaling can be accomplished by moving the cameras in the scene to the correct position, thereby increasing the scale of all virtual objects

- the image presented to the user via a video are shown with their entire view from a certain vantage point, rather than a particular object. they should not undergo transformations like 3d objects do. Instead, the image location must remain locked regardless of how your head is tilted, even as its contents change – following your head movements to mirror what you’d see in real life.

- the user’s eye lenses will remain focused at infinity for headsets like Oculus Rift, so the application must create those depth perceptions instead.

- here are some 3d cinematic tricks to create and reinforce a sense of depth:
    - objects in the distance lose contrast

    - distant objects appear fuzzy and blue/gray (or transparent)

    - nearby objets appear sharp and full color/contrast

    - shadow from hand casts onto objects, especially drop-shadows

    - reflection on hand from objects

    - sound can create a sense of depth

- since headsets like oculus recommends a minimum range of 75cm for objects to be rendered and leap motion tracking range can’t go beyond 75cm, you’ll want to make interactive objects appear within reach, or respond to reach within the optimal tracking rang of the leap motion device

- you may find it that you need to impose additional measures to ensure that objects never get too close to the viewer’s eyes. the effect is to create a shield that protects all moveable objects away from the user.

- there are multiple frames of reference possible in the VR world. here is a list:
    - world frame of reference: object is stationary in the world. as a note, this is the best way to position objects because they exist independently from where you’re seeing it. this also allows computation to be heavily reduced

    - user body frame of reference: object moves with the user, but does not follow head or hands. since an object is following the user body, there may be an instance where an object follows the body but can be also outside the user’s field of view.

    - head frame of reference: object maintains position in the user’s field of view

    - hand frame of reference: object is held in the user’s hand

- lighting, texture, and parallax(the way objects appear to move in relation to each other when the user moves), and other visual features are crucial in conveying depth and space to the user. real-world perceptual cues are always useful in helping the user orientate and navigate their environment.

- latency:
    - reducing latency to the absolute minimum is crucial for development

    - having <20ms latency is needed for optimal head tracking

- unity widgets:
    - button:
        - appears as a discrete element that can easily be distinguished as interactive

        - size and spacing makes it easy for user to press the button and reduce chances of user clicking another button on accident

        - buttons compress in z-space until the are triggered and light up

    - slider:
        - the slider is highlighted when activated

        - indicator lights above the slider change color to create an additional affordance

    - scroll:
        - users can move the content directly rather than attempting to target a small, mouse-style scrollbar

        - the scrollbar within the widget indicates your position within the accessible content.

    - arm HUD:
        - uses a layout that encourages optimal tracking, so that fingers don’t blend into the arts under infrared

        - specific initialization states (turning the arm) ensure that it doesn’t clutter up valuable VR real estate

    - joy ball:
        - The user always has direct control over their motion, preventing motion sickness. When the control is not in use, movement stops immediately

        - Our approach to the interaction pose changed after user testing revealed that it was uncomfortable. Good ergonomics is essential!

        - The Joyball Widget is triggered when hands are between the user and the globe – line of sight is a very useful indicator for determining what the user wants to interact with.

        - Visual feedback ensures that users know how their actions affect the Widget.

- thinking and browsing in 3d space:
    - Many parts of the human brain contribute spatial information to a constantly evolving mental map of our surroundings.

    - with spatial cognition, humans free up more working memory to handle current task at hand

    - humans need space to think

    - space supports human cognitive abilities in a number of ways:
        - spatial semantics:
            - Physical space allows users to spatially arrange objects in order to make sense of data and its meaning, thereby revealing relationships and making connections.

            - The way the space is organized provides the semantic structure we need to make sense of the information

        - external memory:
            - Allowing space for external memory compensates for humans’ limited working memory, allowing people to see more detail and to keep information accessible and visually available.

        - dimension:
            - without thinking, we can immediately tell the differences between two objects based on dimension and other cues.

    - computing is flat:
        - currently, OS works like a series of 2D planes that switch, slide, or blend into each other.

        - this limits our ability to apply our spatial cognition to an application.

        - this complete lack of spatial mapping demands cognitive-heavy task switching from users.

        - this results in every interaction with the OS is an interruption, often requiring many traversals to achieve a goal. some of these things are
            - launching a new app

            - closing an app to move to another activity

            - finding an item

            - accessing the file browser

            - changing windows across apps

            - actions that cause a new window/screen in an app

            - notifications/conversations

        - this reduces productivity
    - bringing spatial cognition into VR
        - Hick’s Law: any interface is vastly improved through the reduction of the number of choices, thereby improving the signal-to-noise ratio.

        - Fitt’s Law: reducing traversal time between objects will naturally improve efficiency

        - both Hick’s Law and Fitt’s Law can be applied to VR/AR

        - VR/AR is inherently spatial

        - comparisons can be done visually, rather than relying on memory and imperfect internal models

        - physical interaction further improved the way users understand and use virtual space, just as it does in real environments
    - the modern browser is a digital task-switching haven, consistenting of built on the tab (resembling a card) and a window(deck of cards)

    - users combine tabs spatially, grouping like tabs into windows

    - these tabs are mapped via a timeline, and a method for keeping track of content, which allows users to:
        - spatially arrange their content

        - put aside a piece of content to revisit later

        - set reminders for necessary tasks/activities  

        - keep their place in a document, even when branching from the initial window

        - engage in parallel browsing across multiple tabs while maintaining multiple back stacks (each tab has its own history)

        - group similar tasks and tabs for sub-tasks (e.g. one window with multiple social networks or emails open)

        - leave page open for a long time over multiple sessions with the intention of returning to them.

        - use greater screen space to open more tabs.

    - tabs thus have spatial presence.
        - the back button can require too many number of clicks to return to a desired page

        - while an open tab maintains state, the back button require the page to reload

        - the browser history requires users to navigate via link name, while tabs allow users to navigate via spatial relationship or visual browsing

    - the restricted space of mobile device screens inhibits access to spatial cognition.

    - browsers often serve as a user’s active memory, and so it is very important that users be able to easily and accurately jump to any given element quickly and reliably.

    - studies show that the more windows and tabs a user has open, the more important the spatial relationships become

    - VR/AR provides the opportunity to increase and improve spatial cognition.

    - AR in particular creates opportunities for users to map their virtual spatial systems to their real ones - opening up rapid development of spatial cognition.

    - the key to a successful spatial browser is a strong baseline grid. we can maintain the existing “launch tab to right” pattern.

    - we also allow users the full reach of their space to organize data using simple drag-n-drop interactions over that baseline grid.

    - no matter what, it is essential that this canvas retain the spatial location of each item until specifically altered by the user.

    - with VR/AR user can maintain “memory tabs” and return to them through spatial memory.

    - dynamically resort objects spatially to reveal meaning.

    - dynamically items sorted png

    - Now that the user can always return to their baseline spatial system, we can capitalize on the digital power of data by providing dynamic spatial semantics.

    - when a user is looking at info, he animated transitions between the views help users understand the context of what they are currently seeing via the animation

    - Microsoft’s example of animation and visual layout: [link](http://research.microsoft.com/en-us/projects/sanddance/)

    - dynamic-dimension ABC png

    - dynamic-dimension Recency png

    - AR/VR offers us the opportunity to create 3D intersections of data visualizations.

    - one way is that visualizations become large and nearer to the user, while items that are not likely to be relevant fall away.In this way, by quickly looking at the dimensions involved, the user can instantly understand the difference between various items – just like in the real world.

    - By unlocking the third dimension, VR/AR opens up the opportunity to combine spatial-cognitive tools and experiences with the raw power and infinite malleability of the digital medium.
