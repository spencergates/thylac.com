---
featured: false
layout: splash
title: "Simple Unix Utilities"
permalink: /unix-utils/
description: "Simple CLI programs written in C to learn low-level systems programming."

header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/media/cli-utils/Tux-Banner.png

excerpt: "Small CLI projects made while learning the C language, and systems programming.

>Created by: Henry Luengas"

video_row1:
  - video_path: /assets/media/cli-utils/simple-tr.webm
    title: "Simple Translate"
    excerpt: "This is a simplified version of the standard \"tr\" utility. It takes as input two sets of characters, then while running it echos STDIN to STDOUT translating any letters in the first input set to the respective letter in the second input set. If only given one set of characters it removes them from the output."
    btn_label: "View Source"
    btn_class: "btn--info"
    url: "https://github.com/HBot106/simple-tr"

video_row2:
  - video_path: /assets/media/cli-utils/simple-timer.webm
    title: "Timer Utility"
    excerpt: "This simple utiltiy takes a number of seconds as input. It then displays a one line timer readout with in the form HH:MM:SS. The timers starts in a running state but can be stopped. An ASCII twirler animates while the timer is running. Hours, minutes, and seconds can be added or removed. When the timer hits zero, the ASCII \"Bell\" notification is played, and the timer will begin counting into negative -HH:MM:SS." 
    btn_label: "View Source"
    btn_class: "btn--info"
    url: "https://github.com/HBot106/simple-timer"
    

video_row3:
  - video_path: /assets/media/cli-utils/simple-20-questions.webm
    title: "20 Questions Game"
    excerpt: "This project is a \"20 Questions\" style game limited to yes/no questions. It uses a binary tree structure to store questions with answers at the leaves. This tree is serialized and desrialized into a text file so that the game can grow after multiple successive playthroughs. If the program guesses wrong, then it prompts the user to add the correct answer and a yes/no question to differentiate it from the program's guess. This new answer will be inserted into the tree for use in subsequent rounds."
    btn_label: "View Source"
    btn_class: "btn--info"
    url: "https://github.com/HBot106/simple-20-questions"
    
video_row4:
  - video_path: /assets/media/cli-utils/simple-make.webm
    title: "Simple Make"
    excerpt: ""
    btn_label: "View Source"
    btn_class: "btn--info"
    url: "https://github.com/HBot106/simple-make"

video_row5:
  - video_path: /assets/media/cli-utils/simple-unix-stats.webm
    title: "Unix System Stats"
    excerpt: ""
    btn_label: "View Source"
    btn_class: "btn--info"
    url: "https://github.com/HBot106/simple-unix-stat"

video_row6:
  - video_path: /assets/media/cli-utils/simple-web-server.webm
    title: "Basic Web Server"
    excerpt: ""
    btn_label: "View Source"
    btn_class: "btn--info"
    url: "https://github.com/HBot106/simple-web-server"

video_row7:
  - video_path: /assets/media/cli-utils/simple-pcap-inspector.webm
    title: "Packet Inspector"
    excerpt: ""
    btn_label: "View Source"
    btn_class: "btn--info"
    url: "https://github.com/HBot106/pcap-packet-info"

video_row8:
  - video_path: /assets/media/cli-utils/simple-chat.webm
    title: "Chat Server & Client"
    excerpt: ""
    btn_label: "View Source"
    btn_class: "btn--info"
    url: "https://github.com/HBot106/simple-chat"


---

<div style="text-align: justify">

{% include video_row id="video_row1" type="right" %}
{% include video_row id="video_row2" type="left" %}
{% include video_row id="video_row3" type="right" %}
{% include video_row id="video_row4" type="left" %}
{% include video_row id="video_row5" type="right" %}
{% include video_row id="video_row6" type="left" %}
{% include video_row id="video_row7" type="right" %}
{% include video_row id="video_row8" type="left" %}


</div>