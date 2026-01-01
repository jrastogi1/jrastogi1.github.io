---
layout: default
title: Projects
permalink: /projects/
---

# LLM Model Serving Analysis (October - December 2025)
As the performance of Large Language Models (LLMs) has improved astronomically for the text generation task since the seminal "Attention Is All You Need" paper in 2017, they have seen widespread adoption across both the corporate and consumer world. These models have a heavy hardware (GPU) requirement, so to keep up with the demand, frameworks for scalable model inference servers (model serving) were developed. The two most common ones today are SGLang and vLLM, and while they optimized input-output operations in different ways, their performance is generally accepted to be equivalent. I collaborated with a group of 4 to benchmark both frameworks, find if there were any differences in lower level metrics, and extrapolate the potential of scalability from the results. 

We used NVIDIA A100s on Microsft Azure virtual machines, organized through Azure Kubernetes Service and Helm charts. We exposed inference metrics through Prometheus and Grafana, and ran load tests through Locust. A sample Grafana result is as follows: 
![Grafana Visualization](../assets/imgs/llm_analysis/Grafana.png)

The metrics we focused on included end-to-end latency (time from an user asking an LLM a question to time of response), requests per second (time needed to process the input tokens), KV Cache usage (how much the models used pre-computed calculations from the attention layers), and more. Some results are as follows: 

![End-to-end Latency](../assets/imgs/llm_analysis/E2E.png)

![Requests per Second](../assets/imgs/llm_analysis/Requests.png)

Based on the results, we determined that while vLLM is faster at low loads, SGLang scales better as the LLM model and user load size increases. We presented our results to Microsoft. 

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
