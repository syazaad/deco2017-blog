---
title: Development and connecting database
date: 2026-05-08
author: SyazaAD
tags:
  - development
  - sql
  - backend
---
This week, I transitioned from planning and wireframing into development. Upon refining the database structure and interaction flow, I started coding the core functionality of the application. The main focus was connecting the frontend pages to the SQL database so trail information could be displayed dynamically rather than hardcoded into the interface.

I began by implementing the Explore page using trail data stored in SQL. Each trail card retrieves information such as trail name, location, difficulty, distance and image URL directly from the database. This was an important step because it changed the application from a static prototype into a functioning system with persistent data handling.

While coding the Explore page, I considered how much information should appear on each trail card. Initially, I wanted to display all available trail details, but this created visual clutter and made the page harder to scan. I decided to prioritise only the most important information for browsing, including the trail name, difficulty and distance. Additional information is displayed only after selecting a trail. This decision improved usability and reinforced the purpose of the Explore page as a discovery tool rather than an information-heavy page.

I also started implementing routing between pages. Users can now move from the Explore page to a Trail Detail page by selecting a trail card. This required passing trail-specific information dynamically rather than relying on separate hardcoded pages for each trail. This approach is more scalable because additional trails can be added to the database without creating entirely new pages.

Another focus this week was preparing the Create Community Hike feature. I started structuring the form and backend logic needed to store hike posts in the database. At this stage, the form includes:

- selected trail reference
- date and time
- meeting point
- optional notes

I intentionally kept the form minimal to reduce implementation complexity and improve usability. Adding features such as participant tracking or organiser profiles would require more advanced backend logic and additional database relationships, which are outside the scope of the prototype.

One challenge during development was understanding how frontend design decisions affect backend structure. For example, displaying community hikes linked to a specific trail requires retrieving data from multiple tables. Overall, this week marked an important transition from conceptual planning into functional implementation. The prototype is beginning to operate as a connected system rather than a collection of mockups. My next step is to complete the "Create Community Hike" flow and test whether users can successfully move from discovering a trail to creating a hike post without confusion or broken interactions.