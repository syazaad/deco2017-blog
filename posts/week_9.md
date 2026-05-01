---
title: Building the trail database
date: 2026-05-01
author: SyazaAD
tags:
  - database
  - sql
  - wireframes
---
This week, upon finalising the wireframe for the Explore page, I started planning the data structure for the hiking trails. Since the Explore page depends on trail cards, I needed to decide what information each trail should include before building the feature.

I began collecting trail data such as trail name, location, distance, difficulty, elevation and image URL. These fields were chosen because they help users compare trails quickly before deciding which one to view in more detail. Difficulty and distance are especially important for users who want to match a trail to their ability.

I then started inputting this data into SQL. This allowed me to move from a visual concept to a more functional system. Instead of hardcoding trail cards, storing them in a database makes the Explore page scalable and easier to manage. I am aiming to collect around 30 trail records. This gives enough variation to test filtering. With only a few trails, filters would not add value. With more data, users can filter by difficulty or distance and get meaningful results.

The next step after collecting this data is to refine the wireframe for the community interaction feature. This includes the page where users can create a community hike or join an existing one. To support this, I need to define what information a hike post requires. This includes:

- trail reference
- date and time
- meeting point
- organiser or creator
- optional notes

This step is important because it connects the trail data to user activity. Without this structure, the core feature of organising hikes would not function properly.

At this stage, I also need to think about how the data connects. A trail can have multiple hike posts, so this introduces a relationship between tables. I do not need a full complex system, but I should aim to clearly define a trails table and hike_posts table linked by trail_id. 

Creating a simple ERD would help visualise this relationship. It also shows that I understand how the system stores and connects data. A full DDD is not required, but outlining key fields and relationships is useful. Basic joins may also be needed later to display hike posts together with trail information.
