---
title: API integration and user testing
date: 2026-05-13
author: SyazaAD
tags:
  - API
  - testing
  - usability
---
Last week during class, we learned about APIs. I focused on evaluating how external APIs and user testing could improve the overall functionality and usability of the application. After developing the core database structure and interaction flow, I started considering features that could make the platform feel more realistic and useful without significantly increasing implementation complexity.

Initially, I considered using a weather API because weather conditions are important for hiking activities. However, after reviewing different API options, I realised that a map-based API would align more closely with the main purpose of the platform. Since the application focuses on discovering trails and organising community hikes, displaying trail locations visually would improve exploration and make the interface feel more interactive.

At this stage, I researched APIs such as Mapbox and OpenStreetMap. The main goal would be to display a map on the Trail Detail page showing the trail location. This would help users better understand where hikes are taking place instead of relying only on text descriptions. I considered the trade-off between functionality and technical complexity. More advanced map features such as live navigation or route tracking would add unnecessary complexity for this prototype, so I decided that a simple embedded map with trail markers would be more appropriate.

I also reflected on how APIs introduce additional responsibilities in development. External APIs require authentication keys, request handling and fallback behaviour if requests fail. This made me consider how the application should respond if map data does not load correctly. Planning for these situations helped me think more critically about reliability and user experience rather than focusing only on interface design.

Another major focus this week was planning user testing and evaluation. Since the main interaction flow of the application is:

- explore trails
- select a trail
- create a community hike

I began thinking about how this flow could be tested with users. One evaluation goal is to observe whether users can move through these steps without confusion or unnecessary actions. If users struggle to locate buttons, understand page transitions or complete the hike creation form, it would indicate usability problems in the design.

I also considered accessibility during testing. The application currently uses a simplified interface with minimal required inputs to reduce cognitive load. Strong colour contrast, readable layouts and consistent navigation are also being prioritised because the application should remain accessible across different user experience levels.

This week helped shift my focus from only building features to evaluating how those features support the overall user experience. My next step is to continue refining the functional flow of the prototype while ensuring the interface remains simple, usable, and technically achievable within the project scope.