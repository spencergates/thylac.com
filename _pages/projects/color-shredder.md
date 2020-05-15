---
featured: true
layout: splash
title: "Color Shredder"
permalink: /color-shredder/
description: "Tie-dye pixel art generation and acceleration"

header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/media/color-shredder/color-shredder-banner-1.png

excerpt: "Tie-dye pixel art from the Color Shredder.

>Created by: Henry Luengas"

feature_row1:
  - image_path: /assets/media/color-shredder/tie-dye.gif
    alt: "Tie-Dye Pixel Art"
    title: "Tie-Dye Pixel Art"
    excerpt: "In this project, I investigated a method for rendering tie-dye like pixel art images. The project was inspired by a Code Golf challenge, \"Images with all Colors\". The goal of the challenge was to make images where each pixel is a unique color. Many algorithms in a variety of languages were submitted, but the images produced by one really caught our eyes. As the poster noted, the produced images look like paintings and are aesthetically interesting. Unfortunately, using the method described takes dozens or even hundreds of hours to create a wallpaper sized HD image, thus it would be completely unfeasible for the even higher resolutions needed for print media. The naive implementation for this process is far too slow to be useful for large images, so I evaluated acceleration of the process using methods including: CPU parallelism, GPU parallelism, just in time compilation, and use of a spatial data structure. The resulting program exceeds the initial scope of the project, but still has ample room for additional improvement. The project successfully generates large, beautiful pixel art tie-die paintings, and served as an excellent instructional tool for learning about parallelization and data structures."  

---

{% include feature_row id="feature_row1" type="left" %}

<a href="https://github.com/HBot106/color-shredder" class="btn btn--success btn--x-large">Download Source</a>
<a href="/assets/documents/Tie_Dye_Pixel_Art_Generation.pdf" class="btn btn--warning btn--x-large">Download Report</a>

![tie-dye](/assets/media/color-shredder/d500-q2-c8-opencl-multi.png)