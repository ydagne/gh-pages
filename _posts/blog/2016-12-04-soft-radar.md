---
layout: post
title: "SoftRadar"
excerpt: "Software Defined Radar"
categories: blog
tags: [sdr, c++, python]
comments: true
share: true
modified: 2016-12-04T14:17:50-04:00
link: https://github.com/ydagne/softRadar
---

SoftRadar is a software defined radio that can transmit and receive (synchronoulsy) radar waveforms. Currently, it targets Universal Software Radio Peripheral (USRP) based hardwares only that support simultaneous Tx and Rx. The main streaming program is written in C++ and is responsible for configuring the hardware, transmitting and receiving radar signals. Some of the hardware settings (frequency, gain, bandwidth,...) are configured via a configuration file. Other real-time controls are handled through a UDP socket for possible remote control. You can download the source code from [here](https://github.com/yDagne/softRadar.git).

SoftRadar can be run from the commnand-line or through a web-interface that can be accessed remotely. Remote access is possible only when the host computer is connected to the network and is visible from the other side where one want to access the radar. Picture below shows snapshot of the graphical interface.


<figure>
	<img src="/images/blog/softRadar1.png" alt="">
</figure>

The graphical interface is also used to upload new waveform file at any time even when the radar is streaming. The device manager records events that occur while streaming. The web interface has a tool that generates a python template code which can be downloaded and modified. The tool is designed as a basis for generating SMPRF radar waveforms. Picture below show snapshot of the interface.


<figure>
	<img src="/images/blog/softRadar2.png" alt="">
</figure>