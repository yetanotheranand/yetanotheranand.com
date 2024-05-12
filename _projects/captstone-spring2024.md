---
name: "Safeguarding User Footprints in Shared Spaces: App-Based Privacy Controls for IoT"
tools: [React Native, Typescript, AWS API Gateway, AWS Lambda, AWS RDS]
image: /assets/images/projects/capstone-spring2024.jpg
description:
external_url:
---

## Problem Statement

The Personalized Privacy Assistant (PPA) project addresses the growing concern over privacy in the Internet of Things (IoT) environment by developing an application that alerts users to the presence and data collection practices of nearby IoT devices, enabling informed privacy decisions and assisting users in exercising control over data collection

## Literature Study

- [Marc Langheinrich](https://link.springer.com/chapter/10.1007/3-540-45809-3_19) introduced a concept for privacy assistants in computing environments, emphasizing the use of beacons alongside service discovery protocols to communicate the privacy policies of data collection services.
- [Das and Sadeh](https://ieeexplore.ieee.org/document/8490188) emphasize the development of privacy assistants aimed at enhancing user control over personal data in IoT environments.

## Design and Implementation

Our overall architecture comprises of three components as mentioned below.

### Beacons and IoT sensors setup

Beacons serve to enhance context-awareness by determining whether an entity is within range.

### Mobile application for sensor discovery

The application periodically scans for beacon signals using the beacon UUID. When a beacon is detected, the application triggers a notification.

### Server to manage IoT infrastructure

- All configuration data related to our IoT infrastructure is stored within a database.
- We provide access to this data through RESTful APIs exposed by our server, allowing the mobile application to fetch information about IoT devices.

{% include elements/figure.html image="/assets/images/projects/SD.svg" caption="Sequence Diagram" %}

## Demo
<div class="w-50">
{% capture carousel_images %}
/assets/images/projects/capstone-demo1.png
/assets/images/projects/capstone-demo2.png
/assets/images/projects/capstone-demo3.png
/assets/images/projects/capstone-demo4-1.png
/assets/images/projects/capstone-demo4-2.png
{% endcapture %}
{% include elements/carousel.html %}
</div>

## Conclusion

- We developed a prototype comprising the described components: beacons, a mobile application, and database hosted on a cloud service provider

- This infrastructure can can be used in libraries and office spaces to minimize the data footprint of outside users when accessing meeting or conference rooms

## Future Work

- Localization of discovered beacons using RSSI or other similar technologies
- Identification of unregistered data collecting devices using their metadata on same wifi or bluetooth network.
- Integrate Machine Learning based techniques to recommend the mitigation strategy based on user’s preference.

## Additional Info

> <a href="/assets/doc/SER517_Team25_ProjectReport.pdf" target="_blank">Project Report</a>

Team Members:
- Ireish Purohit (ipurohi2@asu.edu)
- Atul Prakash (apraka41@asu.edu)
- Anand Gupta (agupt385@asu.edu)
- Anoop Reddy Repaka
- Preetham Akunuri
