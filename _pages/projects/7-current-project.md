---
featured: true
button: "btn btn--success btn--x-large"
layout: splash
title: "Current Project"
permalink: /rusty-color-shredder/
description: "Portfolio website and Rust based Color Shredder compiled into a Wasm web app"

header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/media/color-shredder/color-shredder-banner-1.png

excerpt: "Color Shredder re-written in the Rust language.

>Created by: Henry Luengas"

feature_row1:
  - image_path: /assets/media/color-shredder/tie-dye.gif
    title: "Website & Webapp"
    excerpt: "One important concept that was woefully missing in the Cal Poly computer science curriculum is web-development. So for my latest project I've been working on this website to learn the basics, and display some of my projects. I also felt that my last project, the \"Color-Shredder\", was significantly held back by its python base. Therefore as part of this project I am completely re-writing the project in the Rust language.
    
    
    Rust is a very fast systems language that focuses on near-perfect memory safety. As a result Rust is very useful (though not easy) for implementing multi-processing which was a big part of the color-shredder project. Rust code can also be natively compiled into a web assembly binary since it uses LLVM. So as a final stage of developing this site I want to implement as much of the original project as possible as a Wasm web app.
    
    
    The initial conversion of the basic features to Rust is already complete and working. Now I am learning about how to integrate Wasm binaries with javascript to get the app running here (check back for updates). The rest of the site uses the Jekyll Ruby framework. The basis for this is a Jekyll theme called \"minimal-mistakes\" with many customizations."  

---

{% include feature_row id="feature_row1" type="left" %}

<a href="https://github.com/HBot106/luengas.io" class="btn btn--info btn--x-large">Website Source</a>
<a href="https://github.com/HBot106/rusty-color-shredder" class="btn btn--warning btn--x-large">Rusty Color Shredder Source</a>