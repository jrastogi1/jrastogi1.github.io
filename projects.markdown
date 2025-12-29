---
layout: default
title: Projects
permalink: /projects
---

# LLM Model Serving Analysis (October - December 2025)

TODO brief overview

# Generative Adversarial Attacks on Image Classification (January - May 2025)
In the real world, systems using machine learning models can be adversarially attacked in ways that are visually unnoticable to the users, but cause major changes in model inference. For example, in image classification, a small perturbation to an image can convert the predicted class from "panda" to "gibbon", which can change downstream behavior of the system. In this project, I trained a reinforcement learning agent to generate minimal image-scale perturbations that could reliably adversarially attack a pre-trained YOLOv11 image classifier, trained on the Microsoft COCO dataset, in as few steps per episode as possible. To do so, I used a custom implementation of the Soft Actor Critic algorithm, and the PyTorch and Gymnasium pip packages. This work was novel, since existing RL-based approaches were pixel-based and not generative. Unfortunately, the generation suffered a mode collapse and simply darkened the image, possibly due to the need for reliability. Nevertheless, this was still a good learning experience for RL in application to vision. 

My baseline perturbation was randomly generated noise. Some examples of the results are as follows: 
![Random perturbations](../assets/imgs/gaaic/rand_examples.png)

![Learned perturbations](../assets/imgs/gaaic/learned_ex.png)

My code is publicly available [here](https://github.com/jrastogi1/gaaic). I also wrote a paper and presented this project; the links to both are located [here](https://github.com/jrastogi1/gaaic/tree/main/deliverables). 

# YoloSLAM (January - May 2025)

TODO brief overview

# Robotic Cube Stacker (September - December 2024)

TODO brief overview

# Using Bio-Signals to Predict Smoker Status (January - May 2024)

TODO brief overview
