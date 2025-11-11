---
title: '2.1 Start - Preparation of Installation Package'
date: 2025-11-01
image: images/blake-logo.png
tags: []
description: "Start - Preparation of Installation Package"
iconIdentifier: "bi bi-plus-square-fill-nav-menu"
pageOrder: 1
category: "Using SkyRaom"
quickAccess: 2
---

:::summary
Use the VR template to create a DemoLBE project 
:::

## Use the VR template to create a DemoLBE project 

<p align="center">
  <img src="./images/unity/template.png" alt="Unity VR Template" width="60%"/>
</p>

### 1. Integrate PicoXR
Refer to the Pico Development Website

[Wetsite](https://developer-cn.picoxr.com/resources/) and
[Docs](https://developer-cn.picoxr.com/document/unity/import-the-sdk/)

<p align="center">
  <img src="./images/unity/package.png" alt="package" width="60%"/>
</p>

Add package from git URL

`
https://github.com/Pico-Developer/PICO-Unity-Integration-SDK.git
`

<p align="center">
  <img src="./images/unity/picoxr.png" alt="picoxr" width="60%"/>
</p>

### 2. Nuget
Add package from git URL

`
https://github.com/GlitchEnzo/NuGetForUnity.git?path=/src/NuGetForUnity
`

<p align="center">
  <img src="./images/unity/nuget.png" alt="nuget" width="60%"/>
</p>

### 3. MessagePack
Add package from NuGetForUnity

<p align="center">
  <img src="./images/unity/messagepack.png" alt="messagepack" width="60%"/>
</p>

### 4. System.Text.Json
Add package from NuGetForUnity

<p align="center">
  <img src="./images/unity/json.png" alt="json" width="60%"/>
</p>

### 5. YooAset
Edit/Project Settings/Package Manager
```
Name: package.openupm.com
URL: https://package.openupm.com
Scope(s): com.tuyoogame.yooasset
```

<p align="center">
  <img src="./images/unity/yooaset.png" alt="yooaset" width="60%"/>
</p>

Edit/Windows/Package Manager

<p align="center">
  <img src="./images/unity/yooaset-2.png" alt="yooaset-2" width="60%"/>
</p>

### 6. Add XR Device Simulator

<p align="center">
  <img src="./images/unity/xrsimulator.png" alt="xrsimulator" width="60%"/>
</p>

### 7. LBEMapTool
Add package from git URL
`
https://github.com/OpenLBE/LBEMapTool.git
`

<p align="center">
  <img src="./images/unity/maptool.png" alt="maptool" width="60%"/>
</p>
