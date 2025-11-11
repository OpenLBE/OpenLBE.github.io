---
title: '2.5 Description of the yellow and blue area'
date: 2025-11-01
image: images/blake-logo.png
tags: []
description: "Description of the yellow and blue area"
iconIdentifier: "bi bi-plus-square-fill-nav-menu"
pageOrder: 5
category: "Using SkyRaom"
---

:::summary
3.5 Description of the yellow and blue area
:::

## 1. Blue Zone RecommendAreas
Function: Content Director, used to recommend the best viewing area for users to stand at the corresponding time
Multiple regional settings can be included in a Step, guiding users sequentially to form an exploratory path.

<p align="center">
  <img src="./images/unity/recommend-area1.png" alt="recommend-area1" width="60%"/>
</p>
On the TimeLine, at the same time, the director controls the corresponding area to display
<p align="center">
  <img src="./images/unity/recommend-area2.png" alt="recommend-area2" width="60%"/>
</p>

The position of the area is specified by appending sequence points to LineRender,  note that Use World Space should not be enabled here 
At least three points are required to form a closed convex polygon, and a normal region can be represented by a rectangle with four points. 
Update the appearance, and you can modify the material (Material) DefaultLine of this Lien 
<p align="center">
  <img src="./images/unity/recommend-area3.png" alt="recommend-area3" width="60%"/>
</p>

## 2. Yellow Zone SafeAreas
Function: Content Director, used to limit the user's exploration range. When the user goes beyond this range, the current scene content will disappear, and a prompt will appear to guide the user back to the recommended graph line.
There is generally one yellow area in a Step. 
<p align="center">
  <img src="./images/unity/safe-area.png" alt="safe-area" width="60%"/>
</p>
For the settings of its shape and exterior, you can refer to the blue area. 

## 3. Guide Line
When the user approaches the yellow boundary, the yellow boundary will be displayed; when the user leaves the yellow area, a guiding light column and guiding line will appear. 
Guided attention is the target point where users are expected to return.
The guiding line is the feasible route created based on the current user point and the target point. 
<p align="center">
  <img src="./images/unity/safe-area-2.png" alt="safe-area-2" width="60%"/>
</p>

After replacing resources and entering the guiding space, there will be three Prefabs that can be replaced according to your own content. 
Ground Guide Ground
Guide Light Beam
GuideLine
<p align="center">
  <img src="./images/unity/safe-area-3.png" alt="safe-area-3" width="60%"/>
</p>