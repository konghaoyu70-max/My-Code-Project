# My-Code-Project

## Table of Contents
- [Project Overview](#project-overview)
- [Details](#details)
- [Core Features](#core-features)
- [Preview](#preview)
- [Code Explanation](#code-explanation)
- [Reflection Summary](#reflection-summary)
- [References](#references)



《What's Wrong》 — TunePad Coded Pop Song

Author: Haoyu Kong  

Platform:TunePad  

Project Type: Music Composition  

This project recreates the sound and emotion of Chinese pop music using code instead of traditional recording.  

# Project Overview
This project, titled《What's Wrong》, is a coded Chinese pop track built entirely in TunePad.  

# Details
- Tempo: 110 BPM  
- Key: A Major  
- Time Signature: 4/4  
- Layers:  
  1. Lead Synth Melody  
  2. Electric Piano Chords  
  3. Bass Line  
  4. Drum Pattern  

Each layer exists in its own TunePad cell so it can be edited and tested individually.  
When combined, they perform like a small band.


## Core Features
| Feature | Code Concept | Musical Effect |
|----------|---------------|----------------|
| Melody | `for` loop | Creates a repeated 4-note motif with subtle variation |
| Chords | Lists `[ ]` | Builds triads and harmonic progression |
| Drums | Nested loops + `%` | Generates kick, snare, and hi-hat pattern |
| Bass | Function + `rest()` | Adds groove and spacing |
| Variation | Parameter changes | Adds contrast between verse and chorus |


# Preview

<img width="1321" height="821" alt="截屏2025-10-22 09 43 10" src="https://github.com/user-attachments/assets/b7182da5-1d06-471e-a191-21908d70a187" />


## Code Explanation
Melody:
The melody repeats a four-note phrase three times using a simple loop. Each note’s pitch is a number in MIDI format, and its length is measured in beats. The last note of each phrase is longer to create resolution. On the third repeat, I slightly increased the velocity so the melody sounds more expressive, like a chorus lift. This showed how repetition and variation in code directly shape musical rhythm and energy.

Chords:
The chords use lists to play several notes at once. Each list contains three pitches that form a triad, representing one bar of harmony. By changing the numbers in each list, I could move through a standard pop progression. This demonstrated how data structures can store and control harmonic information in a musical way.

Drums:
The drum part uses nested loops to control timing and a modulus operator (%) to decide when different sounds play. The % alternates between zero and one as the beat counts forward. When it equals one, the snare plays; when it equals zero, the hi-hat plays. This simple rule automatically places snares on beats two and four, creating the familiar pop backbeat while shorter hi-hat notes keep the rhythm light.

Bass:
The bass is built with a function so I can reuse it in different sections. The function takes a list of notes, a beat length, and a velocity, then plays each note with a short rest in between. The small gap adds groove and makes the rhythm feel natural. Adjusting these parameters changes the overall feel of the song and shows how functions make musical patterns flexible and expressive.

# Reflection Summary
Working on this project taught me how code can represent rhythm, structure, and musical emotion. Through loops, lists, and conditionals, I learned to translate musical instinct into algorithmic logic. I realised that programming is not only a technical tool but also a creative medium. It allows precise control over timing and expression while also leaving space for experimentation. Writing this project deepened my understanding of code literacy — the ability to think, design, and communicate through computational structures.

# References
Boden, M. A. (1998). Creativity and artificial intelligence. Artificial intelligence, 103(1-2), 347-356. 

Mateas, M. (2005). Procedural literacy: educating the new media practitioner. On the Horizon, 13(2), 101–111. https://doi.org/10.1108/10748120510608133

Valérie Schafer. (2016). Exploratory Programming for the Arts and Humanities. In WEB90. WEB90. https://doi.org/10.58079/va1j

Paprock. (1992). [Rev. of Mezirow, J. “Transformative dimensions of adult learning” (Book Review)]. Adult Education Quarterly (American Association for Adult and Continuing Education), 42(3), 195. 

Bown, O., Eldridge, A., & McCormack, J. (2009). Understanding Interaction in Contemporary Digital Music: from instruments to behavioural objects. Organised Sound:
An International Journal of Music Technology, 14(2), 188–196. https://doi.org/10.1017/S1355771809000296
