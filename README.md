# Set-Key

The Set key block is used to set the key and mode, eg C Major.
It allows you to change both the mode and key of how solfege is mapped to the notes.

![alt tag](https://github.com/Traitor000/Set-Key/blob/main/set_key2.svg "Set Key diagram")

**Standard Notation of Set Key**

<img width="189" alt="image" src="https://user-images.githubusercontent.com/75945709/184471821-137fd558-2805-4a06-a961-6cbc1505f4be.png">

[RUN LIVE](https://musicblocks.sugarlabs.org/index.html?id=1660313021817245&run=True)

The *Set Key* block will change the key and mode of the mapping
between solfege, e.g., `Do`, `Re`, `Mi`, to note names, e.g., `C`,
`D`, `E`, when in C Major. Modes include Major and Minor, Chromatic,
and a number of more exotic modes, such as Bebop, Geez, Maqam, etc.
This block allows users to access "movable Do" within Music Blocks,
where the mapping of solfege to particular pitch changes depending on
the user's specified tonality.

You can find set key block in the left palette ->  Intervals and then can be used as shown in the above diagram.
In this block to the right, we have two joining points for key {A, B, C, D, E, F, G} and mode {major, minor, lydian, etc.} which can be used to set the key and mode as per requirement.

**Set Key & Movable Do**

Movable Do in combination with the Scale/Mode blocks will transpose sections of music in a nuanced way.
The Set-key block allows you to change both the mode and key of how solfege is mapped to the notes.
For example, in C major - Do is C, Re is D, Mi is E, etc
In F major - Do is F, Re is G, Mi is A.

| Representation | Pitch Movement | Properties |
| --- | --- | --- |
| Movable “Do” | Advanced transposition by mode | Movable Do in combination with the Scale/Mode blocks will transpose sections of music in a nuanced way. |
| | | The Set-key block allows you to  change both the mode and key of how solfege is mapped to the notes. |
| | | For example, in C major - Do is C, Re is D, Mi is E, etc. |
| | | In F major - Do is F, Re is G, Mi is A |

| Representation | Pitch Movement | Properties |
| --- | --- | --- |
| Movable “Do” | Advanced transposition by mode | You also have the option of changing the mode to Minor, Major, Chromatic, and many other exotic modes like hirajoshi, as shown in the example below. |

**Set Key & Scalar step**

**Set Key & Scale Degree**

![alt
 tag](https://rawgithub.com/sugarlabs/musicblocks/master/guide/mode1.svg
 "mode widget")

The *Mode* widget lets you explore modes and generate custom
modes. You invoke the widget with the *Custom mode* block. The mode
specified in the *Set key* block will be the default mode when the
widget launches.




The following chart describes the behavior of different blocks
depending on whether or not a *Movable Do* block is present.

| Block(s) | Fixed or Movable? (Do or La?) | Set Key Transformation? |
| --- | --- | --- |
| Alphabet Pitch | Fixed | No effect. |
| Solfege | Fixed by default  | No effect. |
| Solfege and Movable=Do | Specified via "movable" block set to Do | Yes. |
| Solfege and Movable=La | Specified via "movable" block set to La | Yes. Works like Scale Degree. |
| n^th modal pitch | Movable | Yes. Good for modes of any length. |
| Scale Degree | Movable | Yes. Most useful for 7 note systems. Works just like Movable=La for Solfege by default. |
| Scale Degree and Movable=Do | Movable | Yes. When preceded by Movable=Do, the user can be explicit in their spelling. |
| Scalar Step | Movable | Yes. Navigates up/down within *nth modal pitch* space. |
| Scalar Interval | Movable | Yes. Adds above/under within *nth modal pitch* space. |
| Scalar Inversion | Movable | Yes. Inversion around a specified axis within *nth modal pitch* space. |
| Pitch Number | Movable | No effect. Pitches can be transformed via Set Pitch Number Offset. |
