<p align="center">
  <img src="logo.png" width="140" alt="Afiniel fox logo">
</p>

<h1 align="center">Afiniel Agent</h1>

<p align="center">
  A friendly AI companion for Windows that runs entirely on your own PC and builds 3D models for you in Blender.
</p>

<p align="center">
  <a href="../../releases/latest"><b>⬇ Download the latest version</b></a>
</p>

---

## What is Afiniel?

Afiniel is a desktop chat app, like ChatGPT, except the AI runs **locally** on your own graphics card through [LM Studio](https://lmstudio.ai). Nothing you type is sent to a cloud AI service, and there is no account or subscription.

Ask it to chat, look something up, help with files or code, or **build a 3D model**. When you ask for a model, Afiniel opens Blender, writes and runs the Blender scripts itself, renders the result from several angles, looks at its own renders with a vision model, and fixes what doesn't look right before it shows you.

## Features

- **Chat with local AI models** in LM Studio. Fast, private and free to use.
- **Builds 3D models in Blender**: plans the model, runs each step in a live Blender session, renders previews, critiques its own renders and improves them. Every step can be undone.
- **Opens or installs Blender and LM Studio for you** if they aren't running or aren't installed yet.
- **Web search** and reading web pages, so it can look up things it doesn't know.
- **Weather** for any place, with a 3-day forecast.
- **Files**: reads and writes files in folders you allow. Every change waits for your OK.
- **Runs code** (Python, PowerShell) for calculations and conversions, always shown to you first for approval.
- **Code page**: work on a project folder like a coding assistant, with changes shown as a red and green diff you approve.
- **MCP catalog**: one-click add-ons that give Afiniel more tools (web fetch, Git, time, browser and more).
- **Memory**: remembers short facts about you between chats. You can view, edit or clear them, and use an **incognito chat** that neither reads nor saves memory.
- **Thinking view**: with a thinking model you can watch it reason live before it answers.
- **Models screen**: download recommended models with one click, load and unload them, and give each model its own settings (context length, GPU offload, temperature). It can suggest settings that fit your graphics card.

## Requirements

| | |
| --- | --- |
| **Operating system** | Windows 10 or 11, 64-bit |
| **LM Studio** | Free from [lmstudio.ai](https://lmstudio.ai). Afiniel can install and start it for you. |
| **An AI model** | A vision model, downloaded from inside Afiniel (Settings > Models). Recommended: **Qwen3-VL 30B A3B** for the best results, **Qwen3-VL 8B** for most PCs, **Qwen3-VL 4B** for small graphics cards and laptops. |
| **Graphics card** | NVIDIA GPU recommended. 6 to 8 GB VRAM works with the small model, 12 GB is comfortable for 8B, 16 to 24 GB for the 30B model. It runs without a strong GPU too, just slower. |
| **Blender** (optional) | Only needed for 3D models. Blender 4.2 or newer, free from [blender.org](https://www.blender.org). Afiniel can install it for you. |
| **Disk space** | About 500 MB for Afiniel, plus 3 to 20 GB per AI model. |

## Install

1. Go to the [**latest release**](../../releases/latest) and download the **Setup .exe** under **Assets**.
2. Run the installer.
3. **Windows SmartScreen** will probably say *"Windows protected your PC"*. That happens because the app isn't signed with a paid certificate, not because something is wrong. Click **More info**, then **Run anyway**.
4. Open **Afiniel Agent** from the Start menu or desktop.

## First start

1. **LM Studio**: if the LM Studio pill at the top is red, click it and choose **Start LM Studio for me** (or **Install LM Studio** if you don't have it).
2. **Pick a model**: open **Settings > Models**, choose one of the recommended models and press **Download**. When it's done, select it in the model picker at the top.
3. **Say hi.** Chat normally, or ask for something like *"Make a low-poly treasure chest with gold trim."*
4. **Blender**: the first time you ask for a 3D model, Afiniel opens Blender with its bridge add-on (or offers to install Blender). You can also click the Blender pill and choose **Open Blender for me**.

## Tips

- If replies are slow (the speed under a reply turns amber), the model doesn't fit your graphics card. Try a smaller model, or press **Suggest settings for my GPU** in Settings > Models.
- Each Blender step is one undo step: use **Revert last Blender step** under a render, or Ctrl+Z in Blender.
- Your chats, settings and renders are stored on your PC in `%APPDATA%\Afiniel Agent`.

## Updating

Download the newest installer from [Releases](../../releases) and run it. Your chats, memory and settings are kept.

---

<p align="center"><sub>Afiniel Agent is free to use. The source code is not published in this repository; it only hosts the README and the installer downloads.</sub></p>
