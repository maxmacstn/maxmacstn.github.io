---
layout: page
title: SenseStack
description: Universal IoT hardware platform For Sensor data collection
img: /assets/img/SenseStack/SS_1.png
importance: 1
category: university
---

Following the recent surge of talks about climate change, people have started to care more about the condition of their surrounding environment. These conditions include, but are not limited to, temperature, humidity and pollution level. This phenomenon entails the need to acquire accurate environmental data periodically and as personalized as possible. Despite there being many solutions to perform this task, most are either costly or only accessible to individuals with technical skill or government bodies and large organizations. To answer these challenges, our team proposes SenseStack: an open, extendable environment sensing platform which can provide publicly accessible data or collect private data.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <iframe width="100%" height="400px" src="https://www.youtube.com/embed/lyH1x3b3NAI" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>
</div>
<div class="caption">
    SenseStack introduction video
</div>



To achieve this task, we developed a user-friendly hardware platform for creating sensor nodes which can be configured to suit different environmental sensing tasks with minimal setup. Moreover, our software and hardware are open to modification and extension. In this way, IoT systems become more accessible to a greater span of target users. Our approach consists of an IoT platform based on an ESP32 development board and various sensor modules driven by a megaAVR family microcontroller.

Two key components of the project are the sensor module and main module. Sensor modules, up to ten units per node, sense and repackage environmental data to the main module via a single I2C bus and a data transmission protocol. The main module requests and collects data from the sensor modules, formats them into a JSON packet, and forwards them to a client endpoint IP via POST request. The main module also houses a user interface in which users can setup and configure the node, view live sensor data, as well as update the firmware.

<div class="row justify-content-sm-center">
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/SenseStack/SS_main.png' | relative_url }}" alt="" title="example image"/>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        <img class="img-fluid rounded z-depth-1" src="{{ '/assets/img/SenseStack/SS_sensor.png' | relative_url }}" alt="" title="example image"/>
    </div>
</div>
<div class="caption">
Left, internal of SenseStack Main Module. Right, internal of SenseStack Sensor Module
</div>

Team members
- [MaxMac_STN](https://github.com/maxmacstn) 
- [Tobalation](https://github.com/Tobalation) 
- [CDSW](https://github.com/cdsw)

Project site: [https://github.com/Tobalation/SenseStack/wiki](https://github.com/Tobalation/SenseStack/wiki)

