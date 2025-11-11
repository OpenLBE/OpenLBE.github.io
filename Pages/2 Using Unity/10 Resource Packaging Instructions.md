---
title: '2.10 Resource Packaging Instructions'
date: 2025-11-01
image: images/blake-logo.png
tags: []
description: "Resource Packaging Instructions"
iconIdentifier: "bi bi-plus-square-fill-nav-menu"
pageOrder: 10
category: "Using SkyRaom"
---

:::summary
Resource Packaging Instructions
:::

## 1. Map Information
When the scene/map/Step, etc. changes, MapTool needs to be used to re-export the map information
<p align="center">
  <img src="./images/unity/skyroam-mapfile-2.png" alt="skyroam-mapfile-2" width="60%"/>
</p>

The operating steps are as follows: 
With the Hall scene open, click ImportResources to load all resources under the specified path and stitch them together according to the pre-set orientation. Then click Save Map Config to store the map information. After the completion prompt, you can click Reopen hall Scene to return to the hall scene. 

## 2. Art Asset
When using third-party open-source tools for packaging, please refer to the corresponding official documentation.
https://github.com/tuyoogame/YooAsset
https://www.yooasset.com/
Note:
When there are resource changes, resource packaging needs to be done before releasing the APK.
Menu YooAseet/AssetBundle Builder

<p align="center">
  <img src="./images/unity/yooaset-build.png" alt="yooaset-build" width="60%"/>
</p>
Note to correspond to our URP's choice of ScriptableBuildPipeline