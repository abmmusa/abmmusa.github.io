---
layout: page
title: Research
subtitle: Research projects
---

### High accuracy localization beyond GPS using video analysis
Smartphone GPS receivers typically encounter an error of 10-15 meters under open sky, and over 100 meters in challenging places (e.g., urban canyons), making applications such as navigation for the visually impaired essentially impossible. 
Currently, we are working on a video-based localization solution with sub-meter accuracy using a smartphone’s camera. 
We address three key challenges faced in video-based localization on smartphones. (a) 3D model construction using standard techniques is not robust to the vagaries of smart-phone video, (b) due to resource constraints, 3D model size must be kept to a minimum, and (c) feature extraction, particularly for accurate image features, remains computationally very costly.
Based on an extensive set of both indoor and outdoor videos, meticulously annotated with location ground truth, we demonstrate that our proposed techniques produce accurate models despite challenging video conditions and substantially reduce model size without sacrificing accuracy. 
We also demonstrate an optical-flow based method to reduce the feature extraction effort required for accurate localization.


### Performance and cost optimization for online GPS tracking
For online GPS tracking of mobile devices, optimizing cellular data usage with a controllable error bound is an important problem. 
To investigate real world deployment, we studied a dataset consisting of 1.6 billion GPS points obtained from Nokia Research, and found that 90% are sent using a naive periodic policy (1-300 second period). 
Through experiments we also found that every packet sent incurs significant overhead. 
Additionally, in online tracking, a fundamental three-way trade-off exists among timeliness, accuracy, and data usage. 
With these observations in mind, we designed a thrifty tracking system that allows the user to specify desired targets for any two of timeliness, accuracy, and cost; and optimizes the third. We also provided the first unified view of the three-way trade-off with a closed-form characterization equation.


See more at our [TMC 2016]({{ site.baseurl }}/papers/musa-tmc16.pdf) and and [GIS 2013]({{ site.baseurl }}/papers/biagioni-gis13.pdf) papres.

### Passive localization and tracking using Wi-Fi
All smartphones come with Wi-Fi, and to detect the availability of Wi-Fi networks these smartphones periodically transmit probe messages. 
By deploying Wi-Fi monitors in an area of interest, it is possible to detect these transmissions, providing a coarse-grained location trace for each phone. 
Inspired by these observations, we developed WiFlow to track unmodified smartphones, which enables applications such as monitoring street traffic flow. 
However, some major challenges for passive smartphone tracking are sparse packet transmissions, received signal strength variation, and a variable number of received packets. To address these challenges we used a hidden-Markov-model based solution, using map topology to impose restrictions on movement, and signal strength characteristics. 
Additionally, to obtain more packets from a passing smartphone for improved tracking accuracy, we used low-level Wi-Fi protocol features involving association process and management frames that increased the number of received packets by up to 5 times.


See more at our [SenSys 2012]({{ site.baseurl }}/papers/musa-sensys12.pdf) paper and [SenSys 2011]({{ site.baseurl }}/papers/musa-sensys11-demo.pdf) demo.

### System architecture for large-scale localization and tracking
Designing an efficient computational and network architecture is a challenge for real-time large-scale localization and tracking. 
Smartphones are not fast enough for many computational tasks (e.g., computer vision-based localization described above), and also constrained by limited battery power. 
To address these problems, in collaboration with IBM Research, we are currently developing a framework for offloading computation to edge (e.g., servers connected over Wi-Fi or cellular access points) and cloud nodes. 
This framework distributes application computation across various processing nodes to achieve improved application performance and reduced latency.