---
title: '2.9 Multilingual Settings'
date: 2025-11-01
image: images/blake-logo.png
tags: []
description: "Multilingual Settings"
iconIdentifier: "bi bi-plus-square-fill-nav-menu"
pageOrder: 9
category: "Using SkyRaom"
---

:::summary
Multilingual Settings
:::

## 1. 3.9.1 Resource Preparation
Store the corresponding voice resources in directories according to en-US/zh-CN..., and append them to the AssetBundleCollector.
Pay special attention to setting AddressByFolderAndFileName 

<p align="center">
  <img src="./images/unity/audio.png" alt="audio" width="60%"/>
</p>

## 2. Play
The AudioSource and VoiceSignalReceiver components of the PlayAudio node in the scene are used to receive and play voice 

<p align="center">
  <img src="./images/unity/audio-2.png" alt="audio-2" width="60%"/>
</p>

Append AddVoiceSignalAssetFrom VoiceSignalReceiver to the Timeline, then select the PlayAudio node
<p align="center">
  <img src="./images/unity/audio-3.png" alt="audio-3" width="60%"/>
</p>


Select the sound ID to play, such as 001
<p align="center">
  <img src="./images/unity/audio-4.png" alt="audio-4" width="60%"/>
</p>
