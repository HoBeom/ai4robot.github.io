---
permalink: /air-act2act-en/
layout: splash
title: AIR-Act2Act
header:
  overlay_color: rgba(23,165,137, 0.5)
  overlay_filter: rgba(255, 0, 0, 0.3)
author_profile: false
last_modified_at: 2020-07-13T14:23:03-05:00
toc: true
---

This page introduces Act2Act dataset, a short name for Human-Human Interaction Dataset for Training Robots Nonverbal Interaction Behaviors.

## Introduction

To better interact with users, a social robot should understand the user behavior, infer the intention, and respond appropriately. Machine learning is one way of implementing robot intelligence. It provides the ability to automatically learn and improve from experience instead of explicitly telling the robot what to do. Social skills can also be learned through watching human-human interaction videos. However, human-human interaction datasets are relatively scarce to learn interactions that occur in various situations. Moreover, we aim to use service robots in the elderly-care domain; however, there has been no interaction dataset collected for this domain. For this reason, we introduce a human-human interaction dataset for teaching non-verbal social behaviors to robots. The sample data can be downloaded below and the python scripts to view sample data are available for download at [https://github.com/ai4r/AIR-Act2Act](https://github.com/ai4r/AIR-Act2Act).

Our dataset has the following strengths:

- It is the only interaction dataset of the elderly;
- It provides robotic data to be learned;
- It is one of the largest interaction datasets that provides 3D skeletal data;
- It can be used to not only teach social skills to robots but also benchmark action recognition algorithms.

## Dataset Summary

|Item|Description|
|:--- |:--- |
|Number of samples|5,000 (with three different points-of-view)|
|Number of interaction scenarios|10|
|Number of subjects|100 elderly people, 2 young people|
|Collection environment|1) apartment, 2) senior welfare center|
|Data modalities|RGB video, depth map, body index, 3D skeleton, Robotic data|
|Sensor|Kinect v2|

## Interaction Scenarios

We asked participants to perform each scenario five times. Each interaction scenario is defined as a pair of coordinated behaviors: an initiating behavior performed by an elderly person (E), and a responsive behavior performed by a partner (R). The initiating behaviors consisted of eight greeting behaviors and an additional two behaviors of high-five and hit. The responsive behaviors were designed so that, when performed by service robots, they would be acceptable to people as natural and humble reactions. Since we did not instruct the participants to act in an exact pattern, there were large variations in intra-class action trajectories.

||Interaction Scenario|
|:---: |:--- |
|1|E: enters into the service area through the door.<br>R: bows to the elderly person.|
|2|E: stands still without a purpose.<br>R: stares at the elderly person for a command.|
|3|E: calls the robot.<br>R: approaches the elderly person.|
|4|E: stares at the robot.<br>R: scratches its head from awkwardness.|
|5|E: lifts his arm to shake hands.<br>R: shakes hands with the elderly person.|
|6|E: covers his face and cries.<br>R: stretches his hands to hug the elderly person.|
|7|E: lifts his arm for a high-five.<br>R: high-fives with the elderly person.|
|8|E: threatens to hit the robot.<br>R: blocks the face with arms.|
|9|E: beckons to go away.<br>R: turns back and leaves the service area.|
|10|E: turns back and walks to the door. <br>R: bows to the elderly person.|

## Collection Setup

Our interaction data were collected in an apartment and a senior welfare center where service robots are likely to be used. For each scenario, three cameras were set up at the same height; however, were positioned to capture different views. Two cameras were placed next to each person to capture the behaviors from the point of view of the other person. The last camera was placed in a position where both participants were visible in order to gather information of the participants relative to each other. The position of each camera was adjusted each time to take into consideration the movement range of the participants. In total, the entire dataset has 5,000 interaction samples with three different views, where each view lasts for about 6 s.

- The apartment environment

<img src="http://drive.google.com/uc?export=view&id=1zw33eItZ9xfkwKcP6V6gQLWNmmpAGioT" width="400"/>

- The senior welfare center environment

<img src="http://drive.google.com/uc?export=view&id=1fpmmt8Spu6Wj4UZ83Y3h0Vk_5ZxPNqZw" width="400"/>

## Collected Data

|Data Modality|Resolution|File Format|<center>Size</center>|
|:---: |:---: |:---: |---: |
|RGB video|1920 X 1080|AVI|45.37 GB|
|Depth map|512 X 424|PNG|472.07 GB|
|Body index|512 X 424|PNG|2.12 GB|
|3D skeleton|25 joints|JSON|2.26 GB|
|Robotic data|10 joint angles|JSON|47.0 MB|
|||**Total**|521.88 GB|

## Publication

All documents and papers that report on research that uses the AIR-Act2Act dataset should cite the following paper:

Woo-Ri Ko, Minsu Jang, Jaeyeon Lee and Jaehong Kim,“AIR-Act2Act: Human-human interaction dataset for teaching non-verbal social behaviors to robots," The International Journal of Robotics Research (IJRR), *submitted*.

## Download

Please follow the link below, and join as a member to get to the download page:
- [http://nanum.etri.re.kr:8080/etriPortal/login?language=en](http://nanum.etri.re.kr:8080/etriPortal/login?language=en)

## Contact

Please email wrko@etri.re.kr if you have any questions or comments.

## Acknowledgment

The protocol and consent of data collection were approved by the Institutional Review Board (IRB) at Suwon Science College, our joint research institute.

This work was supported by the ICT R&D program of MSIP/IITP [2017-0-00162, Development of Human-care Robot Technology for Aging Society].
