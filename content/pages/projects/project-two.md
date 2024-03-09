---
type: ProjectLayout
title: Summit Seeker, Efficient High Point Detection in 2D Maps
colors: colors-a
date: '2022-02-20'
client: Awesome client
description: >-
  Embark on a geographic exploration as you are challenged to design an efficient algorithm for detecting the highest point in a 2D map.
featuredImage:
  type: ImageBlock
  url: /images/bg2.png
  altText: Project thumbnail image
media:
  type: ImageBlock
  url: /images/bg2.png
  altText: Project image
---

Objectives:

Develop an algorithm to efficiently identify the highest point on the given 2D map.
Minimize the number of calls to the getElevation(x, y) function as a performance metric.
Showcase algorithmic ingenuity in summit detection.

> “Highest in cohort”

Part 1 - Random Search:
In the initial phase, we allocate a portion of the threshold (0.1%) for Random Search, strategically dividing it into halves for a balanced approach with Local Search.

(a) Uniform Random Search:

Randomly explore the map, ensuring even and uniform coverage across rows and columns.
The search points dynamically adjust to the map's dimensions, enhancing adaptability.
(b) Largest Interval Identification:

Determine the "largest possible interval between points" before Random Search execution.
Identify the coordinate with the highest elevation among the randomly sampled points, crucial for the subsequent Local Search.
Part 2 - Local Search:

Loose Local Search:

Initiate a recursive traversal through neighboring coordinates (top, left, right, and bottom) identified from Part 1.
Conduct a loose local search, leaping across points at intervals of 1% of the map's Height and Width.
Recursively call the traversal function at the highest elevation point discovered, facilitating an in-depth exploration.
Traversal End Conditions:

Terminate the traversal under specific conditions:
Exceeding map range.
Visited coordinates during traversal.
Exceeding the designated search limit for each point.
Worst Time Complexity:
The recursive function demonstrates a worst-case time complexity of O(WH), ensuring efficiency in handling varying map dimensions.

Outcome:
SummitQuest stands as a testament to strategic search methodologies, achieving optimal high point detection with a meticulously crafted algorithm. Our collaborative efforts resulted in the highest recognition within the cohort.

Acknowledgment:
Special thanks to my teammate Tao for the collaborative effort that contributed to the success of SummitQuest.

Visit my github to find out more!
