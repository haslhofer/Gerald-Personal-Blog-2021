---
title: Thoughts on Application Composition
date: "2021-10-27T23:46:37.121Z"
template: "post"
draft: false
slug: "thoughts-on-composition"
category: "Explorations"
tags:
  - "Explorations"
description: "We have moved beyond simply shipping monolithic applications. Here's a short perspective on how mini-apps can be 'composed'"
socialImage: "/media/image-2.jpg"
---
# A basic taxonomy 

    1 - Intermediation
The most invasive strategy is to intermediate other app experiences. The best example is the Google Assistant “sitting on top” of other app experiences and deep linking into these experiences when needed. 

The incentive for the intermediated app is “traffic”, but ultimately, they lose the direct interface to the user and are relegated to be components. It is trivial to conceive other agents that implement the notion of intermediating / observing apps / manipulating other apps.

    2 – Embedding 
Grammarly uses the strategy of embedding itself into other app’s experiences to offer special capabilities (e.g., spelling correction, insertion of content). They are ingredients, often powered by AI. They can be seen as “embedded horizontals”. An OS can offer a standardized extensibility contract (which often exists for input scenarios).

    3 – Aggregation
The aggregation strategy follows the “Mall” model– the anchor store (“Hub app”) leverages its power to attract customers and enables smaller tenants to benefit from the traffic. Apart from navigational convenience (and lower friction in deployment) there is little integration between the apps. The Hub app largely acts like a browser and the apps are websites. There is little benefit in these apps being together given the low level of integration, the main benefit is enabling spillover traffic to tier-2 experiences. Google Docs is one good example of this approach.