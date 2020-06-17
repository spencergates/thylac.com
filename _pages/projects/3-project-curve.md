---
featured: true
layout: splash
title: "Return to the Curve"
permalink: /project-curve/
description: "A 3D platformer game inspired by Marble Blast Gold"

header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/media/project-curve/marble6.png

excerpt: "A 3D platformer game inspired by Marble Blast Gold. Navigate a marble through a series of enemies and obstacles to reach the goal at the end of each level in the shortest time possible!

>Created by: Henry Luengas, Keavon Chambers, Daniel Deegan, Ellen Liu, Connor Virostek"

feature_row1:
  - image_path: /assets/media/project-curve/marble1.png
    alt: "Marble Runner"
    title: "Marble Runner"
    excerpt: "This was a group project for the Real-Time 3D Computer Graphics Software course. In this class we came up with pitches for 3D games and then formed project groups around the most popular ideas. My pitch was Return to the Curve, a Marble Blast Gold clone where the protagaonost marbella has been transported to a strange flat world. Marbella must make it back to her nice curvy world by completeing the levels and avoiding evil cube-bots. Ultimately most of the plot was eventually lost in the rush to implement graphical features for the class, but in the end we ended up with a fun 3 level platformer."   
    
feature_row2:
  - image_path: /assets/media/project-curve/marble4.png
    excerpt: "The Game was implemented in C++ using openGL and contains the following features: 
    
    * Physically-based rendering (PBR) shaders

    * Shadow mapping with supersampling anti-aliasing (SSAA)
    
    * Environment mapping
    
    * Custom physics / collision with arbitrary meshes
    
    * View frustum culling
    
    * Octree spatial data structure (used for collision detection and culling)
    
    * Basic HUD elements"

  - image_path: /assets/media/project-curve/marble3.png
    excerpt: "* Volumetric light beams
    
    * Hierarchically modeled animation
    
    * Positional 3D audio and sound effects
    
    * Bezier curve pathing enemy pathing
    
    * Adjustable 3rd person camera
    
    * YAML level & settings loader
    
    * Platform support for Windows, Mac OSX, and Linux"    

---


{% include feature_row id="feature_row1" type="right" %}
{% include feature_row id="feature_row2" type="left" %}

<a href="https://github.com/HBot106/Project-Curve" class="btn btn--success btn--x-large">Download Source</a>
<a href="/assets/files/curve-builds/curve-windows.zip" class="btn btn--info btn--x-large">Download Windows Executable</a>
<a href="/assets/files/curve-builds/curve-macosx.zip" class="btn btn--info btn--x-large">Download MacOS Executable</a>

<video  style="display:block; width:100%; height:auto;" autoplay="true" muted="true" controls loop="loop">
    <source src="/assets/media/project-curve/Curve_Demonstration.webm"  type="video/webm"/>
</video>


![tie-dye](/assets/media/project-curve/marble2.png){: .align-left}