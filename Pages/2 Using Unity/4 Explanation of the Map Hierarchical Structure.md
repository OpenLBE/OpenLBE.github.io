---
title: '2.4 Explanation of the Map Hierarchical Structure'
date: 2025-11-01
image: images/blake-logo.png
tags: []
description: "Explanation of the Map Hierarchical Structure"
iconIdentifier: "bi bi-plus-square-fill-nav-menu"
pageOrder: 4
category: "Using SkyRaom"
---

:::summary
3.4 Explanation of the Map Hierarchical Structure
:::

## 1. New
The menu SkyRoam/CreateDefaultScene will create a template scene 
<p align="center">
  <img src="./images/unity/createdefaultscene.png" alt="createdefaultscene" width="60%"/>
</p>

will sequentially create a directory named Scene_04 in Scene_01 / Scene_02 /  Scene_03 / to place the newly created scene, which will have a subdirectory named MapPrefab to place the Step prefab. 

<p align="center">
  <img src="./images/unity/createdefaultscene-2.png" alt="createdefaultscene-2" width="60%"/>
</p>

## 2. Node Requirements
In the scene, a Maps node needs to be saved, which is the root node that mounts multiple Steps. 
In Step, Map04_Step01 is the root node of the Step prefab. If the current Step is a vehicle movement, the XTransport component needs to be appended. Refer to the Vehicle chapter 
Start Node, required, the starting point where the current Step stands
End node, required, the end point of the current Step's standing and walking
Map Node, Suggestion, Current Scene Model Mounting Node
SafeAreas node, required, the root node for setting the safety zone of the current Step, append the XSafeAreas component 
RecommendAreas node, required, the root node for setting the recommended walking area of the current Step, append the XRecommendAreas component
TimelineDirector node, required, the animation settings node for the current Step, append the XTimelineDirector component

## 3. Resource Saving
Add the newly created scene, scene Step, and prefab to the AssetBundleCollector of YooAset
<p align="center">
  <img src="./images/unity/createdefaultscene-3.png" alt="createdefaultscene-3" width="60%"/>
</p>
<p align="center">
  <img src="./images/unity/createdefaultscene-4.png" alt="createdefaultscene-4" width="60%"/>
</p>