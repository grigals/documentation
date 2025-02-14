---
sidebar_position: 1
---

# Introduction

Factory+ is an open and modular framework aimed at simplifying and standardising data management across manufacturing organisations. The framework provides a unified approach to data extraction, transport, storage, processing, consumption, and protection, paving the way for future-proofed integration and communication. Factory+ identifies and defines a core set of interconnected components, laying the groundwork for an Industry 4.0 architecture that is well-suited to the modern industrial landscape.

While Factory+ serves as an abstract framework, the AMRC has enhanced its practical application by developing the [AMRC Connectivity Stack](https://github.com/AMRC-FactoryPlus/amrc-connectivity-stack) (ACS). The ACS is a collection of open-source services developed by the AMRC to facilitate a comprehensive, end-to-end implementation of the Factory+ framework. The ACS can be easily deployed onto a new or existing Kubernetes cluster in seconds using Helm, providing a complete solution to start implementing Factory+.

## Motivation & Rationale

The modern factory presents a vision of reduced operating costs, improved sustainability, enhanced productivity, and increased agility, achieved through the intelligent processing of real-time and historical data to gain profound insights into underlying processes and operations. Manufacturers across various sectors are interested in adopting emerging technologies, such as artificial intelligence, big data, IoT, and automation, to take advantage of their transformative potential. By utilising these advanced technologies, organisations can improve their manufacturing processes, increase productivity, reduce costs, and gain a competitive advantage in the rapidly changing industrial landscape. However, some organisations experience a high level of friction and difficulty when adopting digital technologies, while others seem to do so with ease - why?

The missing link lies in solid foundations.

Factory+ addresses the challenges that arise from organic digital architectures that have developed over time, resulting in a complex network of systems that are difficult to utilise, manage, and secure. Factory+ offers a cohesive and future-proofed framework that standardises connectivity and emphasises the establishment of principles, methodologies, and a solid architectural foundation on which to build and implement digital tools.

By implementing a standardised method for machine connectivity, data modeling, data enhancement, and data utilisation, organisations can achieve more flexible data-driven digital processes without the need to start anew each time. By establishing a foundational connectivity standard throughout the organisation and incorporating machine and application connections during the commissioning phase, data access becomes significantly more organised and efficient. Envision trying to operate an online business before the invention of the internet - that's a similar challenge to what many manufacturers face when trying to digitise their operations without having strong, scalable digital infrastructures established.

Numerous industrial devices already possess the capability to communicate using protocols like OPC UA, which may lead to questions about the rationale behind the Factory+ framework and its deviation from this standard. Factory+ and other Sparkplug-based architectures are not designed to entirely supplant technologies such as OPC UA, but rather to supplement them. For instance, OPC UA polling engines are traditionally employed to access raw process variables, which remains the case for Factory+ as well. However, in contrast to transmitting large, bandwidth-intensive poll/response messages through a web of point-to-point connections, Factory+ employs an Edge-of-Network device (Cell Gateway) that only broadcasts encoded Sparkplug messages to all subscribed clients upon detecting a value change. This approach leverages the benefits of report-by-exception, such as reduced data traffic, improved response times, and better anomaly detection, ultimately enhancing efficiency and overall system performance.

Factory+ enables organisations to confidently embrace the potential of Industry 4.0, paving the way for a transformative approach to their manufacturing operations.