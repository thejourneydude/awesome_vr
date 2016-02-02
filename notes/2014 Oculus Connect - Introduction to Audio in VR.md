#### Notes from thejourneydude:


- sound enhances perception of size, space, distance, vection, and smooth object motion.

- sound glues a visual scene together

- specialization and ambience are required to make sound/video work well together

- localization: is the human ability to determine where a sound is coming from
    - if the sound is flat, then this isn’t as strong of a feeling

    - we tell whether a sound if left or right based on the time difference it takes for a sound to reach one ear then the other ear (oversimplified explanation)

    - for sounds top or bottom, our ears can reflect and absorb sounds coming in, and based on the frequencies missing, know if its above or below.

    - head movement helps determine location of sound

    - head, shoulder, and torso filters cues for localization

    - distance
        - for distance, loudness can determine distance, but only if that sound is familiar to us.

        - moving sound sources helps us familiarize us with those new sounds (I assume we can also say sounds we already know too!)

        - initial time delay: having an initial time delay of when you first hear a sound and the reflection of the sound coming from nearby objects helps too

        - mix of direct of and indirect sounds: such as having a friends voice talking to you while other people are surrounding you talking amongst themselves

        - motion parallax: sounds that move quickly across your soundscape, we assume are nearer than further

        - ild: interaural level difference

        - hf damping: high frequency damping isn’t an issue in gaming due to the tight exteriors. That said, the definition is that high frequencies from produced sounds due to humidity and other factors are dampened across long distances

- spatialization: we take what we learn from localization, how do we fake sounds to make it come from a specific position
    - basic methods from pre-vr days:
        - left/right pan

        - front back low pass filter

        - distance volume attenuation

        - no way to shot elevation sounds

        - no head tracking either

    - advanced methods post-vr:
        - direction: hrtfs
            - head related transfer functions. encode filter characteristics for a sound arriving from a specific direction

            - personalized hrtfs can help match sounds to a specific user, but may not work for other users. that said, there are general hrtfs.

            - head tracking helps alleviate the lack luster hrtfs

            - headphones are really really important for sound. they are ideal for using hrtf.

- spatialization only solves direct sound propagation

- ambience provides indirect audio cues. you can pick up if a room is made of tile, wood, size of room. its all based on how sounds bouncing off of surrounding objects

- ambience characteristics:
    - early reflections

    - later reverberations

    - absorption

- spatialization has solved solutions, while ambience needs improvement

- future stuff we need to solve:
    - acoustic raytracing

    - occlusion/diffraction

    - multiband reflection/absorption

    - all of these things above require engine support (all requires access to geometry, etc.)
- sound design
    - monaural sounds will become the norm for 3d positioning

    - sounds should be wide frequency pattern, the more frequencies in a sound the better someone can hear it. having wide frequency helps with spatialization since there is filtering involved in setting spacial location

    - avoid things like sin wave, they are unnatural to a natural setting (assuming you’re putting user in natural sound)

    - sounds must be natural and thus specific to the location. footsteps should come from the feet (a modern hrtf sound?)

- mixing scenes:
    - avoid listener fatigue

    - have slower sounds, helps reduce artifacts

    - audio should match visuals

    - static ambient sounds that aren’t positional can be disconcerting. having ambient noise as positional helps make vr more realistic

    - not everything needs spatialization
        - voiceover, ui, narration, music, low-frequency rumbles like engine noise in a spaceship
- performance implications:
    - you will burn CPU: but with VR focus is just not on graphics, its on immersion

    - graphics latency (10ms+). we are more tolerant of audio latency than graphics latency

    - audio latency (3-100ms+)

    - use native audio format

    - prioritize sounds for spatialization
        - choose n most important

        - avoid spatializating LF sources

        - allow for “2D positioning” path

- oculus going forward is focusing on audio as a first-order priority

- oculus rift audio headphones are set for optimal audio experience (/hailcorporate)

- a problem why headphones haven’t been tackled is the lack of engine support. remember every engine has to handle these audio problems in its own way

- summary: audio is a fundamental part of VR immersion.
