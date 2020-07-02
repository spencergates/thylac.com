---
featured: true
button: "btn btn--primary btn--x-large"
layout: splash
title: "Simple Unix Utilities"
permalink: /unix-utils/
description: "Simple CLI programs written in C to learn low-level systems programming"

header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: /assets/media/cli-utils/Tux-Banner.png

excerpt: "Small CLI projects made while learning the C language, systems programming, and networking.

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
    excerpt: "This project is a simplified version of the extremely usefull unix \"make\" utility, used for compiling multi-file C programs. It starts by opening a \"Smakefile\", and parsing it into a rule tree. The rules for each compilation target, are then processed recurively to compile the program. In this small demo \"example.c\" just takes an argument and calls the factorial function defined in \"fact.h\" and implemented in \"fact.c\". If the \"Smakefile\" is in the propper format the project will be compiled and any relavent errors will be reported."
    btn_label: "View Source"
    btn_class: "btn--info"
    url: "https://github.com/HBot106/simple-make"

video_row5:
  - video_path: /assets/media/cli-utils/simple-unix-stats.webm
    title: "Unix System Stats"
    excerpt: "This program, written for an Operating Systems class, logs system and process stats at a given interval for a supplied executable. In this example the \"glxgears\" demo is run for 5 seconds using a 1 second interval. The logged values are broken into five categories. The obtuse format is a result of the assignment requirements.
    
    
    ### System Time Stats: \n
    userTime, systemTime, idleTime, ioTime, interruptTime, softTime, interruptNum, contextNum, forkNum, runnableNum, and blockedNum 
    
    
    ### System Memory Stats: \n
    memTotal, memFree, memCached, swapCached, memActive, memInactive, 01minuteAvg, 05minuteAvg, and 15minuteAvg
    
    
    ### System Disk Stats: \n
    readsNum, sectorsReadNum, timeReading, writesNum, sectorsWrittenNum, and timeWriting
    
    
    ### Running Process Time Stats: \n
    executableName, state, minorFaultNum, majorFaultNum, userTime, systemTime, priority, nice, threadsNum, virtualMemSize, and residentSetSize

    
    ### Running Process Memory Stats: \n
    totalSize, residentSetSize, sharedPagesNum, codeSize, and dataSize
"
    btn_label: "View Source"
    btn_class: "btn--info"
    url: "https://github.com/HBot106/simple-unix-stat"

video_row6:
  - video_path: /assets/media/cli-utils/simple-web-server.webm
    title: "Basic Web Server"
    excerpt: "This program is an extremely basic and stripped down webserver. It responds only to HTTP/1.0 HEAD and GET querries. It gives error responses for the following scenarios: 400 Bad Request, 403 Permission Denied, 404 Not Found, 500 Internal Error, and 501 Not Implemented. For propperly formed HEAD requests, it responds with the Content-Type and Content-Length. GET requests function in one of two ways. A normal GET request will include the text of the requested file as the body of the response. A GET request to one of the binaries in the /cgi-like/ directory will run that binary and return the text of STDOUT as the body of the response."
    btn_label: "View Source"
    btn_class: "btn--info"
    url: "https://github.com/HBot106/simple-web-server"

video_row7:
  - video_path: /assets/media/cli-utils/simple-pcap-inspector.webm
    title: "Packet Inspector"
    excerpt: "This program will read and inspect packet data from, \".pcap\" files captured by other programs such as wireshark. For all packets, the Ethernet header info is printed. Next, either IP or ARP headers are read and printed. Finally, for any IP packets, the TCP, UDP, or ICMP header info gets read and printed. For TCP and UDP packets commonly used ports for services like HTTP, DNS, FTP, TELNET, SMTP, and POP3 are also checked and reported. TCP packet checksums are calculated and compared to the header value, to check for malfored or corrupt TCP packets as well."
    btn_label: "View Source"
    btn_class: "btn--info"
    url: "https://github.com/HBot106/pcap-packet-info"

video_row8:
  - video_path: /assets/media/cli-utils/simple-chat.webm
    title: "Chat Server & Client"
    excerpt: "This client-server chat program allows many users to sign on to a chat server, and send private messages between one another or public broadcasts to all users. It uses a custom built message packet, that is encapsulated and sent over the network as a TCP packet. Both the client and server can recieve, interpret, and send these packets to facilitate the chatting system. The client program interacts with the user, allowing them to \"sign-on\" with a handle and message other registered handles, or all connected users. The server recieves, checks the valididty of, and passes the messages to their intended recipeint(s). It also manages the registration and deregistration of user handles as well as providing clients with the list of available users. In this small demo, three clients register handles and demonstrate some of the chat features." 
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