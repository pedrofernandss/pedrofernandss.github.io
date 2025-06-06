---
title: "The Traveling Salesman Problem: From Gregor Samsa to Max Verstappen in the Incessant Search for the Perfect Route."
meta_title: ""
description: "this is meta description"
date: 2025-05-29T05:00:00Z
image: "/images/gallery/post01/cover.png"
categories: ["Computer Science", "Algorithms"]
author: "Pedro Fernandes"
tags: ["algorithms", "formula 1"]
draft: false
---

A traveling salesman is a person who constantly travels to different cities and regions in order to sell products on behalf of a company. You may or may not remember, but a famous example of a traveling salesman is the character Gregor Samsa, from The Metamorphosis. Gregor worked hard as a traveling salesman to support his family and pay off his parents' debt, having an exhausting routine and facing various pressures at work.

As a traveling salesman is a seller who needs to pass through several locations, there is a need to choose the best route to save time. For this, there are two basic factors that need to be considered: the distance between cities and the order in which they are visited. In addition, we also need to consider that the traveler should not pass through the same location twice.

On a small scale, it is possible to solve this problem easily. Observing the illustrative image below, we can see that some locations have exits to two other cities while some have an exit to only one city. Something relatively common, according to reality.

{{< image src="https://dev-to-uploads.s3.amazonaws.com/uploads/articles/9vw7vft4qzvf1d3qj1ww.png" caption="" alt="alter-text" height="" width="" position="center" command="fill" option="q100" class="img-fluid" title="image title"  webp="false" >}}

Imagine the first path is:

**Rio de Janeiro, London, Cape Town, Moscow → Resulting Distance: 70 km**

Now if we travel:

**Cape Town, Moscow, London, Rio de Janeiro → Resulting Distance: 90 km**

Both paths meet the proposed requirements, however, the second path is longer, more costly, and more tiring for the traveling salesman. One way to discover the best path is simply by testing all possible possibilities and combinations, something plausible to do in small situations. However, despite seeming like a simple problem, as the number of locations to be visited increases, it becomes more difficult to find good solutions. And this proved to be a real nightmare for many mathematicians and computer scientists.

But okay, now you might be wondering what Max Verstappen 🦁 have to do with the traveling salesman. Well, both of them dislike traveling long distances unnecessarily.

> I’ve always said that we have too many races on the calendar. But I think the bigger problem is traveling across different time zones, between Las Vegas and Qatar. We are flying to the other side of the world again and I think we can do a slightly better job on the triple-headers, that they are a bit closer together. For me, that would make a bit more sense, so that’s probably something we need to look into - Max Verstappen

For those who don't know, Max Verstappen is a four-time Formula 1 world champions with Red Bull. And by 2025, the F1 championship is set to have 24 Grands Prix, meaning it will holds races in 24 different cities, passing through 21 countries and 5 continents.

With society's growing awareness regarding sustainable development, the environmental impacts caused by industry, the greenhouse effect, the zero Carbon footprint, etc., one of Formula 1's biggest difficulties has been finding the best and most efficient organization of races throughout the year to reduce the enviroment impact without creating conflicts with the sponsors because, despite what many believe, the greatest environmental impact caused by the organization comes from travel (whether by sea, air, or land) while the emissions from racing cars account for only 0.7%.

Returning to the computational theme, on this large scale and with great distances, trying to find the best solution by calculating and testing all possibilities would be extremely exhaustive. Observing the table below, with just 24 cities the number of possibilities becomes impossible to calculate by hand and extremely long for a simple computer.

| Cities      | Possible Combinations |
|-------------|-----------------------|
|      1      | 1           | 
|      2      | 2           |
|      3      | 6           |
|      4      | 24          |
|      5      | 120         |
|      6      | 720         |
|      7      | 5040        |
|      8      | 40320       |
|      9      | 362880      |
|      10     | 3628800     |
|      11     | 39916800    |
|      12     | 479001600   |
|      24     | 620448401733239439360000   |

And even though, in the 1980s, researchers Grötschel, Padberg, Rinaldi managed to solve the problem with up to 2392 cities, the Traveling Salesman Problem remains more relevant than ever. Some argue that hardware evolution is the main solution to current computational problems, to the point where we no longer need to worry so much about algorithm optimization. However, we can reflect and observe from history that problems like the traveling salesman and its discussion over the years have brought solutions that were applied in the most diverse areas. Therefore, even if hardware evolution is a great advancement, the construction of intelligent solutions to problems is equally important.

With each new F1 season, with its global calendar, or with each logistical challenge that arises, the need to find the most intelligent route persists, with researchers constantly developing methods to deal with the growing complexity of the real world.

After all, who knows, maybe in a while we will need to find the best routes between galaxies, stars, and planets? 🚀
