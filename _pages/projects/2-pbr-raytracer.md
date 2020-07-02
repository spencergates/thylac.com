---
featured: true
button: "btn btn--primary btn--x-large"
layout: splash
title: "PBR Raytracer"
permalink: /pbr-raytracer/
description: "Raytraced PBR video renderer with basic kinematic motion"

header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/media/raytracer/pbr-banner.png

excerpt: "Raytraced PBR video renderer with basic kinematic motion.

>Created by: Henry Luengas"

feature_row1:
  - image_path: /assets/media/raytracer/pbr-2.png
    alt: "PBR-GI"
    title: "PBR Raytracer"
    excerpt: "This was a solo class project for Advanced Rendering Techniques. In this class I built a raytracing image renderer. It parses as input a subset of the POV-Ray scene description language and renders the scene. The rendering equation uses a Cook-Torrance BDRF and accounts for reflection, refraction, occulsive shading, Fresnel's law, and Beer's law. Planes, triangles, spheres, and boxes are all suppported and can use matrix transformations. Multiple lights are supported and a spatial data structure is used to cut down on ray-object intersection checks. Global Illumination is achieved through Monte-Carlo samlpling and the renderer supports super sampling anti-aliasing. Finally gravity is implemented into the scene along with sphere-plane collision physics, to render multilple successive frames. The frames are passed to FFmpeg to be compressed into an output video. Each frame is rendered using CPU multiprocessing for a modest speedup." 


---

{% include feature_row id="feature_row1" type="left" %}

<a href="https://github.com/HBot106/simple-pbr-raytracer" class="btn btn--success btn--x-large">Download Source</a>

<video  style="display:block; width:100%; height:auto;" autoplay="true" muted="true" controls loop="loop">
    <source src="/assets/media/raytracer/simple-pbr-raytracer.webm"  type="video/webm"/>
</video>

![pbr1](/assets/media/raytracer/pbr-1.png)

