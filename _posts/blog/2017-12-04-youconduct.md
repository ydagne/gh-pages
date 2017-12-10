---
layout: post
title: "Youconduct (Virtual orchestra)"
excerpt: "A python script that allows you to conduct a virtual orchestra"
categories: blog
tags: [python opencv]
comments: true
share: true
modified: 2017-12-04T14:18:26-04:00
link: https://github.com/ydagne/youConduct
---


<figure>
	<img src="http://www.trbimg.com/img-53e3e2cc/turbine/la-ca-0928-salonen-pg" alt="">
</figure>



**YouConduct** is a small python project that allows you to conduct an orchestra of virtual instruments. **YouConduct** is based on two libraries: [**fluidSynth**](http://www.fluidsynth.org/) and [**OpenCV**](https://opencv.org/). **FluidSynth** is a software that synthesizes music in real-time from a soundfont file. **OpenCV** (Open Source Computer Vision Library)  is known for its powerful real-time graphics processing capabilities. The code is available on [github](https://github.com/ydagne/youConduct).

In order to use youConduct, you need to install the following libraries first:

  - fluidSynth 
  - opencv2
  - python binding for opencv

For debian distributions, you can install the above as follows:

```bash
sudo apt-get install libopencv-dev python-opencv fluidsynth
```
  
# colorSound.py

**colorSound** lets you conduct a virtual orchestra using colors. It processes images captured from a webcamera and tracks three colors (Green, Blue, and Red). **colorSound** uses the **OpenCV** library for image processing and tracking of colors. When you run the script, it shows a video stream captured from your camera. Currently, **colorSound** detects and tracks three colors. Only one instance of each color with largest size is tracked, and each color plays different instrument. The soundfont that comes with youConduct (`soundFont1.sf2`) has three instrument presets. 

  - Green - Yamaha Grand Piano
  - Blue - Violin
  - Red - Ahh Choir


<iframe width="560" height="315" src="https://www.youtube.com/embed/zS5q4DHf4qs" frameborder="0" gesture="media" allow="encrypted-media" allowfullscreen></iframe>


Just grab anything that has at least one of the three colors and conduct the orchestra as professionals do. The software can play three instruments simultaneously if it sees all the three colors. Colors can be detected from your shirt too!

You can play other/more instruments by modifying the script to use different soundfont file. If you use different soundfont, make sure that you select the appropriate `program` and `bank` for each instrument. 
