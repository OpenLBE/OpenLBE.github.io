---
title: '2.3 Scene Description'
date: 2025-11-01
image: images/blake-logo.png
tags: []
description: "Scene Description"
iconIdentifier: "bi bi-plus-square-fill-nav-menu"
pageOrder: 3
category: "Using SkyRaom"
---

:::summary
Scene Description
:::

## 1. Hall Scene
Description: The entry point of the entire project, the location where users stand and prepare after entering the game.
Function:
There must be one and only one node with the component XEntryPoint, which is the starting position of the entire game, defaulting to (0, 0, 0). 
Launcher node, the entry point for the project startup script, is mandatory.
Node VideoPlayer_Plane, plays the opening 2D video, not required. 
Node VideoPlayer_360 plays the opening 3D video, which is non-essential. 

## 2. Level Scene
Note: For the content experience level scenario, a unified path will be placed. Taking Demo as an example, the placement directory is as follows for reference 
Use the menu SkyRoam/MapTool to open the MapTool tool and set the path 

<p align="center">
  <img src="./images/unity/maptool-file.png" alt="maptool-file" width="60%"/>
</p>

```
Assets\Samples\Dubnium.LBEBuilder\X.Y.Z\Starter Assets
---------------------------------------\Scene_01
---------------------------------------\Scene_01\Scene\Scene_01.unity
---------------------------------------\Scene_01\MapPrefab\Map01_Step01.prefab
---------------------------------------\Scene_01\Timeline\Scene_01_Step01_Timeline.playable
---------------------------------------\Scene_02
---------------------------------------\Scene_02\Scene\Scene_02.unity
---------------------------------------\Scene_02\MapPrefab\Map02_Step01.prefab
---------------------------------------\Scene_02\Timeline\Scene_02_Step01_Timeline.playable
```

Scene naming convention: Scene_XX, where XX is a two-digit number used to identify the scene order.
Naming convention for steps (Step): MapXX_StepYY, where XX can correspond to the scenario number, and YY is a two-digit number indicating the Step order. 
In a scene, according to production requirements, there can be [1-N] Steps to sequentially form a scene. 
The subdirectories Scene and MapPrefab are fixed and not allowed to be modified. 

## 3. Scene Switch
On the Timeline track, simply append NextStepAsset at the transition point
<p align="center">
  <img src="./images/unity/timeline.png" alt="timeline" width="60%"/>
</p>