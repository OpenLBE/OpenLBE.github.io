---
title: '2.8 Description of the Avatar Character'
date: 2025-11-01
image: images/blake-logo.png
tags: []
description: "Description of the Avatar Character"
iconIdentifier: "bi bi-plus-square-fill-nav-menu"
pageOrder: 8
category: "Using SkyRaom"
---

:::summary
Description of the Avatar Character
:::

## 1. The default image is the Unity robot 
Assets\Samples\Dubnium.LBEBuilder\Version\Starter Assets\Prefab\RobotKyle.prefab
The avatar can be replaced by substituting this prefab (  RobotKyle ) 

## 2. Replace with new resources
Example  https://www.mixamo.com/  Download Michelle as an example to perform character replacement, with at least two actions: Idle and Walk 

<p align="center">
  <img src="./images/unity/mixamo.png" alt="mixamo" width="60%"/>
</p>

Requirements for the newly created character Michelle.prefab.
### 1. Append the Animator component to the root node, 
Mount a written AnimatorController, which defines two parameters
Speed: The speed range is represented as [0, 1], where a value of 0 indicates standby and a value of 1 indicates walking
Height: The height range is represented as [-1, 1], where a value of -1 indicates squatting and 1 indicates normal standing
 The example is a simple BlenderTree, and content providers can set it according to their own content. 
<p align="center">
  <img src="./images/unity/player-2.png" alt="player-2" width="60%"/>
</p>
### 2. Mount a TMP_Text
Mount a Canvas/Name, which will be used to display the user's name. If this component is not present, the name will not be displayed. 
<p align="center">
  <img src="./images/unity/player-1.png" alt="player-1" width="60%"/>
</p>

### 3. Set Tag and Layer
Set Tag to Player, Layer to Ground
<p align="center">
  <img src="./images/unity/player-4.png" alt="player-4" width="60%"/>
</p>

### 4. More precise control 
Open the Resources/Dubnium_Config file, and you can modify the configuration of the corresponding role inside, as follows
There are two corresponding forms, walking mode and wheelchair mode. Each mode corresponds to a prefabricated body of a different gender. You can replace the default by dragging the prefabricated body you made to the corresponding position.
If only one Michelle is used as the default, the Default Avatar can be changed to Michelle, which is RobotKyle by default. 

<p align="center">
  <img src="./images/unity/player-3.png" alt="player-3" width="60%"/>
</p>