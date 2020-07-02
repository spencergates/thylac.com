---
featured: true
button: "btn btn--primary btn--x-large"
layout: splash
title: "Fortnite Disco"
permalink: /fortnite-disco/
description: "OpenGL animation projects"

header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/media/fortnite-disco/fortnite.jpg

excerpt: "Three small OpenGL animation projects.

>Created by: Henry Luengas"

video_row1:
  - video_path: /assets/media/fortnite-disco/tie-fighter.webm
    alt: "Part 1"
    title: "Key Frames, Quaternions, & Curves"
    excerpt: "The first OpenGL program is a keyframe animated scene of a Tie-Fighter chasing the Millenium Falcon through a scene. The goal of this program was simply to learn about and use keyframe-animation, interpolation, quaternions, and splines. The program allows the user to fly around the space and record keyframes recording the camera's position and orientation. Three of these sets of keyframes were applied to the three scene models (2 ships, and the camera). Quaternions are used for smooth rotation interpolation. The spline and terrain rendering was provided by an instructor." 

video_row2:
  - video_path: /assets/media/fortnite-disco/facial-animation.webm
    alt: "Part 2"
    title: "Facial Animation"
    excerpt: "In my second OpenGL animation project, a wireframe face is animated to articulate some user provided text. The goal of this project was to gain some familiarity with animating the vertices of a model rather its position or orientation. There are 10 different variations of the basic face model made in blender to represent several mouthshapes corresponding to verious basic phonetic sounds.  The text is read at a constant rate and a rudimentary descion tree picks the current and next mouthshapes to animate between." 

video_row3:
  - video_path: /assets/media/fortnite-disco/fortnite-disco.webm
    video_caption: "Unmute for music."
    alt: "Part 3"
    title: "Character Animation & Animation Blending"
    excerpt: "In the final part of the class I was ready to tackle the initial goal and create a Fortnite disco. The first challenge in doing this was extracting the models and animations from the encrypted Fortnite game files, thankfully decryption keys gathered from a memory dump of the runnig game were availble from many anonymous sources online. The next step was converting the skeletons and their animations to the autodesk FBX format. The FBX-SDK was used to read FBX animation files into a skeleton (bone-tree) data structure; this conversion functinality was provided by the instructor. Each skeleton has 2 idle animations, a forward and backward walking animation, and 12 dance animations. Funtionality is provided for rendering the skeleton while interpoalting the aniamtions from Idle to Walking and back to Idle and from Idle to Dancing and back to Idle. This is just about everything needed to realize the initial goal; however, the two person dance off became a single person performance due to time constraints. Also the rendering of the character models were abandoned in favor of rendering the skeleton so that model skinning wouldn't have to be accounted for. In the final scene, the character walks up, strikes his idle pose, then goes through each of his dances a few times, blending into and out of idle between each." 


---
Fortnite Disco was my final project for a 3D animation course. The initial goal of the project was to make a disco scene where two 3D characters compete in a dance off. I intended to use models and the animations from the unreal engine game “Fortnite”. This ended up being a bit too ambitious of a goal, but I learned a lot about animation along the way.


{% include video_row_autoplay id="video_row1" type="left" %}
{% include video_row_autoplay id="video_row2" type="left" %}
{% include video_row_autoplay id="video_row3" type="left" %}


