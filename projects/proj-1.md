---
layout: post
title: 'Sonic Sculptural Staircase in Head-Mounted Augmented Reality'
---
### Yichen Wang, The Australian National University
### [Henry Gardner](http://users.cecs.anu.edu.au/~Henry.Gardner/), The Australian National University
### Matt Adcock, Data 61, CSIRO
### [Charles Martin](https://charlesmartin.com.au) (Project Lead), The Australian National University

## Abstract

We present an interactive sound art work, Sonic Sculptural Staircase, that delivers a sonic experience to enhance the appreciation of a sculptural staircase and its surroundings in a head-mounted augmented reality system. Our work includes ten different interactive sonic features with visual overlays to incorporate the staircase for users to explore. We describe the design and implementation of our system and provide a demo video of it in use.

{% include image.html url="https://youtu.be/LfUVl-848U0" image="projects/proj-1/thumb.jpg" %}


### Author Keywords

augmented reality, sonic art, architecture, sculpture, HoloLens

### CCS Concepts
•Applied computing→Arts and humanities→Sound and music computing;•Applied computing→Arts and humanities→Media arts; •Human-centered computing~Human computer interaction (HCI)~Interaction paradigms~Mixed / augmented reality

## Introduction 

Sonic Sculptural Staircase is a head-mounted augmented reality (HMAR) sound artwork that integrates sound, visual overlay and interaction to enhance the appreciation of a sculptural staircase and its surroundings. The work designed ten different interactive sonic features that mainly exploits sound as the main information channel to prompt the user’s engagement and convey the meaning behind the staircase.

The work is realised with [Microsoft HoloLens 2 Augmented Reality(AR) headset](https://docs.microsoft.com/en-us/hololens/hololens2-options?tabs=device) and was programmed based upon the 3D staircase model as holograms in [Unity](https://docs.unity3d.com/2019.3/Documentation/Manual/index.html). The work explored two different types of sound: context-related recordings and electronic sound,  that combines interaction and visual into AR holograms to present an immersive experience.

{% include image.html image="projects/proj-1/holo.jpg" caption = "Microsoft HoloLens 2"%}

Previous work in this field has achieved a personalised sonic experience that incorporates real-world features. By embedding sound sources in AR holograms (that model the physical environment), one can directly access the information as well as engage with [a sculpture](https://arxiv.org/abs/2012.02311). Such installations not only augment the user’s experience but also provide a new practice of using sound in HMAR. Other sonic applications in HMAR such as [Augmented Piano](https://www.nime.org/proceedings/2020/nime2020_paper80.pdf) and [INVISO AR](https://www.nime.org/proceedings/2020/nime2020_paper24.pdf) have explored visual overlays to assist music composition and performance.

Recent advancements that integrate so-called ‘instinctual interaction’ into HMAR systems enable vivid tactile experiences, allowing the touch, grasp, and movement of virtual objects like one would with real objects as well as [interactive aural sensations and feedback](https://docs.microsoft.com/en-us/windows/mixed-reality/design/interaction-fundamentals). These HMAR affordances advance the interactive potential of mixed reality environments and allow further integration of interactive sound, and visuals. 

In this paper, we describe our sound artwork Sonic Sculptural Staircase that reflects the new development progress in HMAR as well as how sound can be utilised with interaction in a real-world setting. We first introduce the aesthetic background and description of the user experience in our work. We then discuss the design details of interactive sonic features in this sound artwork. We conclude our work by providing a video-demo that illustrates our design.

## Sonic Sculptural Staircase
Sonic Sculptural Staircase is created upon a staircase at the Hanna Neumann Building at the Australian National University (ANU). The work was designed to be triggered by sonic interaction and walking within the staircase to enhance people's awareness of its aesthetic context. Sound is exploited as the main information channel to covey meaning during this experience. Our sound sources are categorised to three themes: 1) mathematics-related sounds (e.g., chalkboard sketching sound) 2) computer science-related sounds: (e.g., keyboard typing sound) 3) sounds appearing in the building that map the aesthetic context or the occupants working environment (e.g., swipe-card sound).

### Aesthetic Context

The staircase is located at the Hanna Neumann building at the Australian National University, [part of the School of Computer Science, Mathematical Sciences Institute and the Statistical Consulting Unit in ANU](https://maths.anu.edu.au/news-events/news/keeping-hanna-neumann’s-legacy-alive-new-hn-building). Cryptographic and brick patterns surround the building's interiors and architecture to [reflect the heritage and culture behind](https://www.worldarchitecturenews.com/article/1588290/coded-building-hanna-neumann-building-australian-national-university). The staircase at the centre of the building is an interface linking the mathematics and computer science faculties. It was designed in the sculptural form with the concept of a [“collaborative stair”](http://clarkekeller.com.au/projects/learning/anu-computer-science-mathematical-sciences-in/) embedding the message of collaboration across disciplines.

## Design and Development

As illustrated in the feature map below, ten different interactive sonic features are placed deliberately at different parts of the staircase.  These features enable the user to have different views of the building’s interior with sonic information mapped to the real-world context. 

{% include figure.html image="projects/proj-1/feature.jpg" caption="Feature Map" %}

### Description of User Experience

The Sonic Sculpture Staircase experience starts at the front of the staircase on level 2 where a large swirling button is present. When the user pushes the button, a ‘‘level 2’’ sound is played with text message ‘‘Welcome to Sonic World!’’ popping up. Walking through the button, the user approaches the staircase. While walking up the staircase, sci-fi-like sounds are played with ascending pitches and an immersive swirl appears on top of the stairs. 

When the user arrives at the level 2.5 platform, a hand icon shows up at three locations inviting the user to explore interactive sonic features. These features are a raining sound with virtual raindrops coming down in front of the window; a sketching chalkboard sound in front of the mathematics department’s physical chalkboards; and a coffee machine sound near a virtual coffee cup. At the opposite wall, a keyboard sound is played over a virtual “matrix code” effect.

Continuing to walk up the stairs towards the computer science department,  piano notes are played as the user moves. At the top of the stairs, ‘‘level 3 and going down’’ is played to indicate the experience has finished, although the user can go back and continue interacting.

## Sonic Interactive Feature

### Feature Details
The below table shows Sonic Sculptural Staircase feature details. The design of each feature considers sound, interaction and visual aspects which discussed at the below section.

 |    |       Feature Name       |        Sound/Sonic       |      Interaction       | |            Visual             |
|----|:------------------------:|:------------------------:|:-------------:|:--------------:|:-----------------------------:|
|    |                          |                          | Intentional   | Unintentional  |                               |
| 1  | “Welcome to Sonic World” |   Swapping card sound    |        √      |                |       Button-like swirl       |
| 2  |        “Going up”        |  “Level 2” & “Going up”  |               |       √        |         Stage colored         |
| 3  |    Sci-Fi sound making   |   Sci-fi sound pitches   |               |        √       |         Stage colored         |
| 4  |    Sci-Fi sound making   |   Sci-fi sound pitches   |        √      |                |         Changing color        |
| 5  |  “Feel the rain inside”  |      Keyboard typing     |        √      |                |         Matrix effect         |
| 6  |    Chalkboard Writing    |    Chalkboard writting   |       √       |                | Chalk powder spreading effect |
| 7  |         “Matrix”         |   Coffee machine sound   |       √       |                |          A coffee cup         |
| 8  |        Coffee Time       |        Rain drops        |       √       |                |           Raindrops           |
| 9  |      Crushing Piano      |        Piano notes       |               |        √       |         Stage colored         |
| 10 |       “Going down”       | “Level 3” & “Going down” |               |        √       |                               |

### Interactions

Two types of interaction: intentional and unintentional, are designed to address both users' engagement and context sensitivity for the appreciation of the staircase and the building.

Intentional interaction, refers to interactions that requires the user to actively engage with the staircase. These are prompted by visual stimuli. For example, Chalkboard Writing requires the user to place their hand near the railing to trigger the corresponding sound source. Unintentional interaction refers to the interaction triggered simply through the user’s presence.

### Sounds 

Three sonic material included in this work relate to mathematics (e.g. chalkboard writing), computing (e.g., keyboard typing ), or the working environment and aesthetic context of the building (e.g., swipe-card sounds). Two types of sound sources: context-related and electronic are used in this installation.  The context-related sound sources were pre-collected in the Hanna Neumann building using an audio recorder. The electronic sound is generated in real-time using the Disunity Synthesiser Toolkit ([DisunityST](https://github.com/digego/DisunityST)), a C# audio  library focussed on enabling audio synthesis implementations in Unity. DisunityST is used to generate sci-fi-like sounds in feature 4 in the table.

## Implementation Details

The experience was realised using a Microsoft Hololens 2 AR headset and programmed in Unity version 2019.3.7.f1. The Microsoft's [Mixed Reality Toolkit (MRTK)](https://github.com/microsoft/MixedRealityToolkit-Unity) and [World Locking Tool (WLT)](https://microsoft.github.io/MixedReality-WorldLockingTools-Unity/README.html) have been applied during the sonic experience development to design location-specific sonic interactions. The implementation contains three steps. First, the real-world staircase was modelled in [Cinema4D](https://www.maxon.net/en/cinema-4d) based on its physical structure and used as holograms. The 3D staircase model is composed by series of child holograms(Step 1). Second, the staircase model was manually aligned with the physical staircase using WLT (Step 2). Third, sound sources, visuals and interactions are integrated to specific child holograms to realise ten different sonic interactive features in Unity (Step 3). Hand interactions are achieved with MRTK while presence interactions use collision detection scripts written in C# in the Unity back-end environment.

{% include figure.html image="projects/proj-1/original.png" caption="Original Staircase" %}

{% include figure.html image="projects/proj-1/c4d-2.PNG" caption="Staircase model in Cinema4D" %}

{% include image.html url= "https://youtu.be/LUOdZrxvUxs" image="projects/proj-1/c4d-2.PNG" caption="Step 2: Aligning Staircase Model in Real-world" %}

{% include figure.html image="projects/proj-1/unity.PNG" caption="Step 3: Sonic Sculptural Staircase Experience Development in Unity" %}


## Conclusion

We created an interactive sound art installation on a sculptural staircase using the HoloLens 2 HMAR system. Our work explored different combinations of sound, interaction and visuals to present an immersive experience. Our exploration of an HMAR sonic experience in a real-world location could provide useful insights into how Sonic Interaction Design can contribute to sculptural spaces and how new musical instruments can make use of HMAR platforms.

Our preliminary findings with users indicated that our sonic experience is compelling in terms of the sense of immersion by visual overlays, especially large ones that surrounds users. While the experience of individual interactive sonic features such as feature 6 or feature 7 in the given table are relatively isolated in a sense that they have weakened the immersive experience as a whole. These findings encourage us to pursue further studies including, a formal user evaluation, to examine the immersive experience demonstrated by our work.
