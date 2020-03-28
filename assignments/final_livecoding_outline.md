

<!--
Jennifer Notes:
- Why these dimensions?
- Reduce dimensions to about 6-7
  - Learning barriers for newcomers / musical expressiveness for expert live coders
  - Choose ones that you can evaluate, or present in prior literature
-->



# An Analysis of Live-Coding Systems
*Mert Toka*
*MAT 594X - Final Project*

### Abstract
This paper analyzes and compares four live-coding systems to find affordances and limitations of each system.   

### Introduction
In its broader definition, live-coding means any programming activity that is written and executed almost simultaneously. Therefore, it is not bound to a specific domain and it refers to any real-time software development. However, in the recent years, the term started to appear in the context of improvisational sound and visual production through real-time programming. 

Over the years, there has been many programming languages and systems that supports different affordances for improvisational creative programming. This document focuses on a subset of these systems, and analyzes them on two perspectives: (1) the affordances of each system and their support for various modalities; (2) an investigation of their support for cognitive dimensions of notation [1]. 

I selected the systems in this analysis based on my personal familiarity with the tools:
- Gibber [2] is a web-based live-coding language that supports native web audio synthesis and visual elements 
- SuperCollider [3] is a server-client program for high-fidelity audio synthesis
- TidalCycles [4] is a pattern programming language built on a functional programming paradigm for robustness and easy pattern manipulation
- Siren [5] is a hybrid system that merges textual and visual programming for live-coding with an additional interface
  
Each of these systems are being developed as an open-source project.

### Background
- the role of algorithms in music production
- rhythm and repetition
- patterns
- creative computing and live-coding / history
- text-editors / IDEs / CLIs

### Methodology
I compare each system based on the state of the software (Table 1) and their cognitive dimensions for notational systems [1] (Table 2). 

**Table 1:**
||Gibber|SuperCollider|TidalCycles|Siren|
|--- |--- |--- |--- |--- |
|Underlying Programming Language|Javascript, GLSL|SClang|Haskell|SClang, Haskell|
|Learning Curve|Moderate|Steep|Easy|Moderate|
|Support for Visual Elements|Full Integration|None|None|Moderate Integration|
|Support for Web Browsers|Online|None|Supports|None|
|Complexity of Installation|Trivial|Easy|Moderate|Hard|
|Robustness|Robust|Fragile|Robust|Robust|

**Table 2:**
five-point Likert scale

|Cognitive Dimension||Gibber|SuperCollider|TidalCycles|Siren|
|--- |------ |--- |--- |--- |--- |
|Visibility | How easy is it to view and find elements or parts of the music during editing?|4|1|3|4|
|Juxtaposability | How easy is it to compare elements within the music?|3|2|3|3|
|Hidden Dependencies |How explicit are the relationships between related elements in the notation?|2|2|2|4|
|Hard Mental Operations | When writing music, are there difficult things to work out in your head?|5|1|4|5|
|Conciseness / Diffuseness | How concise is the notation? What is the balance between detail and overview?|3|2|2|2|
|Provisionality | Is it possible to sketch things out and play with ideas without being too precise about the exact result?|5|5|5|5|
|Secondary Notation |How easy is it to make informal notes to capture ideas outside the formal rules of the notation?|5|5|5|5|
|Consistency |Where aspects of the notation mean similar things, is the similarity clear in the way they appear?|5|5|5|5|
|Viscosity|Is it easy to go back and make changes to the music?|5|5|5|5|
|Role Expressiveness|Is it easy to see what each part is for, in the overall format of the notation?|5|5|5|5|
|Premature Commitment|Do edits have to be performed in a prescribed order, requiring you to plan or think ahead?|5|5|5|5|
|Error Proneness|How easy is it to make annoying mistakes?|2|5|1|2|
|Virtuosity / Learnability|How easy is it to master the notation? Where is the respective threshold for novices and ceiling for experts?|4|1|4|3|
|Abstraction Management/ Extensibility|How can the notation be customised, adapted, or used beyond its intended use?|3|5|2|2|
<!-- |Closeness of Mapping|Does the notation match how you describe the music yourself?|3|1|2|3| -->
<!-- |Progressive Evaluation (Audibility / Liveness)|How easy is it to stop and check your progress during editing?||||| -->

### Evaluation
An individual investigation of each system is presented in following sub-sections.

- People
  - Musicians
  - Visual Artists
  - Programmers
- Text Editor
  - Syntax
  - Shortcuts
  - Highlighting
- Interface Features
  - Visualization/Annotation
  - Plugins/extensibility
- Dissemination Strategies
  - Examples
  - Tutorials

#### Gibber
*Gibber* is an audiovisual live-coding environment for web browsers developed by Charlie Roberts in 2012 [2]. It supports Javascript and GLSL as its main programming languages, for audio and visual programming, respectively. It synthesizes audio using Web Audio API and renders visual components with shaders in WebGL. 

// Add examples of the syntax

The interface consists of multiple views. First and most important component is the text editor. 

// Add screenshots

#### SuperCollider
*SuperCollider* contains an environment and a programming language for real-time audio synthesis and algorithmic composition. It has been developed by James McCartney and released in 1996 [3]. It uses a server-client architecture that separates the language and audio synthesis. The server, SCserver, interfaces the programming language, SClang, and provides a powerful and robust audio generation. It does not have a visual component.

// Add examples of the syntax

SuperCollider is not developed as a live-coding environment. However, along with offline algorithmic composition, its robust server also supports improvisational audio generation. Specifically `PBind` class makes pattern generation and event dispatching easier by enabling repetitions and discrete step structures.  

The open-source nature of the software enables various plugins, called Quarks, to be developed for additional features. For example, `SuperDirt` is a sampler added to SuperCollider to be able to use audio samples efficiently with   

// Add screenshots



#### TidalCycles
One of the prominent figures in live-coding history, Alex McLean, developed and released *TidalCycles* (*Tidal*, in short) in 2009 as a pattern language [4]. It is a pattern language because it does not synthesize audio by itself; it communicates with SuperCollider server through Open Sound Control (OSC) and triggers samples or synths. The syntax of the Tidal, however, enables an economic use of  It uses a simplified version of Haskell functional programming language for its syntax.

// Add examples of the syntax

// Add screenshots

#### Siren

// Add examples of the syntax

// Add screenshots


### Discussion
- compare and contrast different modalities 
  - web
  - visual
  - programming paradigms
- possible guidelines for improved workflows based on the findings

### Conclusion
- potential directions
- summarize results
- opportunity areas for a new/improved software

### References
[1] - Nash, C. (2015). The cognitive dimensions of music notations.

[2] - Roberts, C., & Kuchera-Morin, J. (2012). Gibber: Live coding audio in the browser. In ICMC.

[3] - Wilson, S., Cottle, D., & Collins, N. (2011). The SuperCollider Book. The MIT Press.

[4] - McLean, A., & Wiggins, G. (2010). Tidal–pattern language for the live coding of music. In Proceedings of the 7th sound and music computing conference.

[5] - Toka, M., Ince, C., & Baytas, M. A. (2018). Siren: Interface for pattern languages. In Proceedings of the International Conference on New Interfaces for Musical Expression (NIME) (Blacksburg, Virginia, USA, 2018), TM Luke Dahl, Douglas Bowman, Ed., Virginia Tech (pp. 53-58).



___
## Prompt
#### Analyzing Existing Technologies: 

Perform a critical analysis of a field of established creative technologies. Provide evidence for the limitations and opportunities of these technologies and propose concrete directions for future development of alternatives. Your analysis should include the following elements: 

a. A description of the domain of technologies/ tools that you have chosen to focus on.

b. A description of a minimum of 5 exemplar technologies drawn from HCI/ systems research publications or prominent examples used in real-world practice. Note: these can include technologies discussed in class.

c. An exploration of the affordances and qualities of these example technologies that connects their features and constraints to the kinds of things that can be made with them and / or the people who can use them. You may choose to use charts or visualizations to map out this space.

d. A following section that advocates for a new tool or technology that targets a space that has not been explored by the existing tools in your analysis. Note: The new technology you propose in the essay need not be a technology you’re working on (though it could be). Think of this as an exercise in identifying opportunities and articulating the differences between systems, not in describing what you’re actually building.





Visibility  &  How easy is it to view and find elements or parts of the music during editing? &
Juxtaposability  &  How easy is it to compare elements within the music? &
Hidden Dependencies  & How explicit are the relationships between related elements in the notation? &
Hard Mental Operations  &  When writing music, are there difficult things to work out in your head? &
Conciseness / Diffuseness  &  How concise is the notation? What is the balance between detail and overview? &
Provisionality  &  Is it possible to sketch things out and play with ideas without being too precise about the exact result? &
Secondary Notation  & How easy is it to make informal notes to capture ideas outside the formal rules of the notation? &
Consistency  & Where aspects of the notation mean similar things, is the similarity clear in the way they appear? &
Viscosity & Is it easy to go back and make changes to the music? &
Role Expressiveness & Is it easy to see what each part is for, in the overall format of the notation? &
Premature Commitment & Do edits have to be performed in a prescribed order, requiring you to plan or think ahead? &
Error Proneness & How easy is it to make annoying mistakes? &
Virtuosity / Learnability & How easy is it to master the notation? Where is the respective threshold for novices and ceiling for experts? &
Abstraction Management/ Extensibility & How can the notation be customised, adapted, or used beyond its intended use? &