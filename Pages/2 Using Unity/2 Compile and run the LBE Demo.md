---
title: '2.2 Compile and run the LBE Demo'
date: 2025-11-01
image: images/blake-logo.png
tags: []
description: "Compile and run the LBE Demo"
iconIdentifier: "bi bi-plus-square-fill-nav-menu"
pageOrder: 2
category: "Using SkyRaom"
---

:::summary
Compile and run the LBE Demo.
:::

## 1. Import DemoUsage & Starter Assets

<p align="center">
  <img src="./images/unity/maptool-2.png" alt="maptool-2" width="60%"/>
</p>

Double Click Hall Scene
<p align="center">
  <img src="./images/unity/hallscene.png" alt="hallscene" width="60%"/>
</p>

Set Hall Use Start Scene
<p align="center">
  <img src="./images/unity/hallscene-2.png" alt="hallscene-2" width="60%"/>
</p>

## 2. Resource Allocation
Click Menu [YooAsset/AssetBundle Collector]
<p align="center">
  <img src="./images/unity/yooaset-config.png" alt="yooaset-config" width="60%"/>
</p>
Click Button Import 
<p align="center">
  <img src="./images/unity/yooaset-config-import.png" alt="yooaset-config-import" width="60%"/>
</p>

Select MapTool Demo file [\Assets\Samples\Dubnium.LBEBuilder\1.0.3\Demo Usage\Config\AssetBundleCollectorConfig.xml]
<p align="center">
  <img src="./images/unity/yooaset-config-import-2.png" alt="yooaset-config-import-2" width="60%"/>
</p>

Click Menu [YooAsset/AssetBundle Builder] And Click Build.
<p align="center">
  <img src="./images/unity/yooaset-build.png" alt="yooaset-build" width="60%"/>
</p>

## 3. Set SkyRoam Configuration
Click Menu [SkyRoam/Platform Settings] And Click Build.
<p align="center">
  <img src="./images/unity/skyroam.png" alt="skyroam" width="60%"/>
</p>

Contact us, and you will receive an APPID for development and deployment. During the debugging phase, you can set it to 00000000-0000-0000-0000-000000000000

<p align="center">
  <img src="./images/unity/skyroam-2.png" alt="skyroam-2" width="60%"/>
</p>

## 4. Configure the map relationship information of the example project
Click Menu [SkyRoam/MapTool] And Click Build.
<p align="center">
  <img src="./images/unity/skyroam-mapfile.png" alt="skyroam-mapfile" width="60%"/>
</p>

Click button [Select resource folder] ,select [Assets\Samples\Dubnium.LBEBuilder\1.0.3\Starter Assets\SceneAssets]
<p align="center">
  <img src="./images/unity/skyroam-mapfile-2.png" alt="skyroam-mapfile-2" width="60%"/>
</p>

Click button [Import Resource] ,select [Assets\Samples\Dubnium.LBEBuilder\1.0.3\Starter Assets\SceneAssets]
<p align="center">
  <img src="./images/unity/skyroam-mapfile-3.png" alt="skyroam-mapfile-3" width="60%"/>
</p>

Click button [Save Map Config]
<p align="center">
  <img src="./images/unity/skyroam-mapfile-4.png" alt="skyroam-mapfile-4" width="60%"/>

</p>
Click button [Reopen Hall Scene]

## 5. Android Keystore Information Configuration
```
ANDROID_KEYALIAS_NAME=demo
ANDROID_KEYALIAS_PASS=passworld
ANDROID_KEYSTORE_PASS=passworld
ANDROID_KEYSTORE_PATH=c:\Users\dev001\Keystone.jks
```

## 6. Compile the APK of the Demo
Set CompanyName & ProductName & Version
<p align="center">
  <img src="./images/unity/setting.png" alt="setting" width="60%"/>
</p>

Uncheck Override Default Package Name, then Package Name will be com.CompanyName.ProductName,
Demo is com.Qumeta.DemoLBE

<p align="center">
  <img src="./images/unity/setting-2.png" alt="setting-2" width="60%"/>
</p>

Click Menu [SkyRoam/BuildApk] And Click Build.
//DemoLBE\Builds\Android\DemoLBE_YYYYMMDD_HHmmss.apk
Under normal circumstances, a compiled demo apk will be obtained