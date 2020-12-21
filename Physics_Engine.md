# Developing a Game Physics Engine
***

Have you ever wondered how the objects you see in games interact with each other? How collisions between different physical bodies is simulated in real time? All of it has to do with how the Physics Engine is written! With a well written physics engine, you can accurately simulate the movement and collision of bodies with each other according to Newtonian Physics. The aim of this project is to develop such a physics engine in JavaScript.

### Disclaimer
You will not need to write a rendering engine for this physics engine. A project for writing rendering engines would be completely different from this. You will simply be writing through a buffer to an HTML5 canvas, to read up on canvas in HTML5, visit: [Canvas](https://www.w3schools.com/html/html5_canvas.asp)

## Prequisites
- ### JavaScript
  JavaScript provides easy rendering capabilities by writing to an html canvas, which you can launch directly to your browser. This, of course, will not give you free access to your discrete graphics card for rendering larger and more complex scenes, if you have one. (Look into a little thing called OpenGL for that). JavaScript has a fairly different syntax from the C++ you learn in CS101, so for resources on that, look up [JavaScript](https://www.w3schools.com/js/default.asp)

- ### Basic Physics Engine
  You will learn how a basic physics engine is written, where to start, what concepts you need to understand etc. A general layout of the concepts would look like:
  - Understanding Motion Dynamics
  - BroadPhase Collision Detection
  - NarrowPhase Collision Detection
    - Implementing GJK (The Gilbert-Johnson-Keerthi Algorithm) if possible
  - Impulse resolution for collisions
  
## Resources and Aim
The main aim of this project would be to build a working physics engine. To test this physics engine, you can build different test scenarios or go on to develop an entire game with it, although that would be outside the scope of this SoC (A ModelViewController approach is recommended for that, follow this [tutorial](https://youtu.be/w-OKdSHRlfA) and related [code](https://github.com/frankarendpoth/frankarendpoth.github.io/tree/master/legacy/content/pop-vlog/javascript/2018/006-rabbit-trap)). 

Given resources can be referred to, in order:
1. [Build a basic game engine in JS](https://www.graphitedigital.com/blog/build-your-own-basic-physics-engine-in-javascript)
2. [Motion Dynamics](http://buildnewgames.com/gamephysics/)
3. [Broad Phase Collision Detection Using Spatial Partitioning](http://buildnewgames.com/broad-phase-collision-detection/)
4. [GJK Algorithm](https://disq.us/url?url=https%3A%2F%2Fmollyrocket.com%2F849%3AlCXtetgf9YHMt7wShspF19n5pMw&cuid=1308141)

In case you are finding it difficult to bridge the gaps between any of these parts (especially 2-3-4), look at [this](http://allenchou.net/game-physics-series/). The implementation in this is in C++, but has things written in much more detail. You can also follow the entire project through this link! (Provided you put in the work to translate from C++ to JS).