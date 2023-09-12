# Zindi-Network-traffic-project

# Project Description

Traffic scenario classification can be used in multiple service scenarios to accurately optimize network parameters or take different management and control measures based on the specific scenario. For example, in intelligent operation and maintenance, different fault types can be identified based on the traffic performance caused by each fault. 
In intelligent congestion control, rate control parameters can be configured based on traffic performance to ensure high throughput, low delay, and no packet loss. However, the status parameters of traffic in different scenarios may not differ significantly due to limitations in the collection device. Moreover, the number of scenarios within a given duration is uncertain, and random switching between scenarios can make it difficult to identify them. In some real-time decision situations, a response time of milliseconds or even microseconds may be required, which presents a greater challenge in solving the problem.

During transmission and forwarding processes, network traffic may be sent to the same port queue by multiple ports. As the output rate of the forwarding device is limited by the port bottleneck bandwidth, the input rate of traffic is higher than the output rate, resulting in the need for the forwarding device to allocate cache space to store burst traffic. This creates a cache queue at the egress port of the forwarding device. The queue length in the cache queue changes based on different types of forwarding traffic.

Currently, some status parameters, such as input rate (v_in), output rate (v_out), real-time length of the cache queue (q), and corresponding time (t), are collected at fixed time intervals. The output rate (v_out) is limited by the port bottleneck rate (v_max) where v_out <= v_max, while the input rate is affected by the burst and regulation protocol. So the maximum of input rate may be higher than the bottleneck rate. Here, the input and output rates are measured by the amount of traffic received and sent during each fixed time interval.

# Problem Statement

The objective of this challenge is to build a model based on the training set data to predict the traffic scenario for unknown traffic at each moment.
Note: In this context, "unknown scenario" refers to a scenario with known traffic but unclear which of the known scenarios it belongs to, rather than a completely new scenario that has never occurred before.

This project is a competition on Zindi by Ai for Good
AI for Good is organized by ITU in partnership with 40 UN Sister Agencies. 
The goal of AI for Good is to identify practical applications of AI to advance the United Nations Sustainable Development Goals and scale those solutions for global impact. 
It’s the leading action-oriented, global & inclusive United Nations platform on AI.
