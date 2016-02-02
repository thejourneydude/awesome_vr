####Notes from thejourneydude:

- Vergence accommodation conflict: the way that the lenses of your eyes focus on an object is totally separate from the way that your eyes physically aim themselves at the object you’re trying to focus on.

![Vergence Accommodation](https://cdn-images-1.medium.com/max/1600/1*BRB4QLpT7bxA5QZN3d2xrA.jpeg)

- What complicates things further is how long it takes your eyes to adjust their vergence in order to look from
near-field to far-field. it takes a long time to focus from a near object to a far sided object

- Current-gen HMDs for virtual reality are a flat square screen inside a pair of goggles that simulate depth of field. There is a disparity between the physical surface of the screen (vergence) and the focal point of the simulated world you’re staring at (accommodation).

- Fortunately, there are some good best practices in virtual reality UX design that we can use to reduce or avoid VAC-induced discomfort.

- some possible solutions include hardware changes, light fields, or writing code to account for these kinds of effects.

- there are a couple of UI VR recommendations that one can follow:
    - use long viewing distances when possible: focus cues have less influences as the distance to the display increases. beyond 1 meter should suffice

    - match the simulated distance in the display and focal distance as well as possible. that means place in-game objects being examined or interacted with in same range as simulated static focal point.

    - move objects in and out of depth at a pace that gives the user’s eyes more time to adjust. moving object fro close to far away or vis very can be more tiring to the eyes than not

    - maximize the reliability of other depth cues.  Accurate perspective, shading realism, and other visual cues that convey realistic depth help take a cognitive load off brains already coping with VAC. Note: simulated blur falls into this category, but current approaches to blur effects tend to exacerbate the negative impacts of VAC, ymmv.  (I believe tech will solve this by next gen.)

    - minimize the consequences of VAC by making existing conflicts less salient. Try not to stack multiple smaller objects at widely-varying depths overlapping each other, especially not when your users will be viewing them head-on for an extended period of time. Also try to increase the distance to the virtual scene whenever possible.
