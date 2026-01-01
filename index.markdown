---
layout: default
title: Homepage
---

<!-- Launch with `bundle exec jekyll serve --baseurl=""` -->

# Welcome!
Hi, I'm **Jai Rastogi**, a third year undergraduate at University of Maryland - College Park. I specialize in computer vision, robotics, and reinforcement learning, and am passionate about experimenting with and challenging the boundaries of today's technology for real-world applications. Basically, I like to make robots and machine learning models work, find ways to make them suck, and iterate again! Explore my portfolio to see my projects, and feel free to connect with me through the contact page!

## Work Experience
* Machine Learning Intern @ Pacific Northwest National Laboratory (June - December 2025)
* Machine Learning Research Intern @ DEVCOM Army Research Laboratory (June - August 2024)

## Featured Projects
A more comprehensive list of projects is located [here](/projects/). 

### [LLM Model Serving Analysis](/projects/#llm-model-serving-analysis-october---december-2025)

As the load on large language models (LLMs) scales, it becomes necessary for the LLM servers to optimize model inference to return responses as quickly as possible. The two most popular frameworks for this purpose today are SGLang and vLLM, and are widely considered to give equal performance. My group was mentored by a Principal Software Engineer at NVIDIA, and we defined 'better performance' as capability to scale. After benchmarking both on NVIDIA A100s with load tests through Azure virtual machines, we determined that SGLang scales better, and presented our results to Microsoft. This provided valuable experience into Cloud Computing, and LLM benchmarking and analysis. 

### [Generative Adversarial Attacks on Image Classification](/projects/#generative-adversarial-attacks-on-image-classification-january---may-2025)

In the real world, systems using machine learning models can be adversarially attacked to change model inference results, such as deleting detections of a person in a surveillance camera. These attacks can cause bad actions or actors to go unnoticed, which can have major consequences. In this project, I trained a reinforcement learning agent to adversarially attack a pre-trained YOLOv11 image classifier using a novel generative approach. While it ultimately yielded poor results, it was a good learning experience. 

### [YoloSLAM](/projects/#yoloslam-january---may-2025)

Simultaneous Localization and Mapping (SLAM) systems enable robots and related devices to both create a map of their environment and pinpoint their location within it, and are essential for operation in unknown environments. They see use in drones, smart vacuum cleaners, self-driving cars, and everything in between. All current SLAM approaches analyze the environment by comparing distinctive points, such as corners and edges, to each other. In this project, I developed an algorithm to compare object detection results instead, mimicing the human approach to SLAM. While it assumes a static scene, it provides a step towards human level scene analysis. 