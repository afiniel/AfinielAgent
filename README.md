<p align="center">
  <img src="logo.png" width="140" alt="Afiniel fox logo">
</p>

<h1 align="center">Afiniel Agent</h1>

<p align="center">
  A powerful personal AI agent for Windows that runs entirely on your own PC. It researches, writes, plans, works with your files and code, runs tasks for you, and even builds 3D models in Blender.
</p>

<p align="center">
  <a href="../../releases/latest"><b>⬇ Download the latest version</b></a>
</p>

---

## What is Afiniel?

Afiniel is your own AI agent, like ChatGPT or Claude, except the AI runs **locally** on your own graphics card through [LM Studio](https://lmstudio.ai). Nothing you type is sent to a cloud AI service, and there is no account or subscription.

It doesn't just answer. Give it a task and it uses its tools to get it done: it searches the web and reads sources, writes and edits documents, plans multi-step work, does exact math, reads and edits your files, writes and runs code, and checks its own work before it tells you it's finished. Anything that changes your files or runs on your computer waits for your OK.

And when you want something in 3D, Afiniel opens Blender, writes and runs the Blender scripts itself, renders the result, looks at its own renders with a vision model, and fixes what doesn't look right.

## Features

- **A real agent**: plans bigger tasks step by step, uses tools, checks the results and fixes what failed.
- **Research**: web search and reading pages, with sources. Big research jobs go to a helper agent with its own fresh context.
- **Writing and planning**: emails, documents, summaries, translations, study and project plans, ready to copy (it can put text on your clipboard).
- **Files**: reads, searches and edits files in folders you allow. Every change is shown as a diff and waits for your OK.
- **Runs code and commands** (Python, PowerShell) for data, conversions and automation, plus long-running jobs like dev servers in the background. You approve each one.
- **Code page**: a coding workspace in the style of Claude Code, with compact tool steps, inline diffs, numbered permission prompts, a file tree, a changes list and a terminal.
- **Exact math and time zones**: a built-in calculator and clock, so numbers and dates are right.
- **Opens things for you**: links in your browser and files in their default app.
- **Builds 3D models in Blender**: plans the model, runs each step in a live Blender session, renders previews, critiques its own renders and improves them. Every step can be undone.
- **Long chats stay sharp**: older parts of a long chat are summarized automatically, so the model keeps the full picture.
- **Memory**: remembers short facts about you between chats. You can view, edit or clear them, or use an **incognito chat**.
- **MCP add-ons**: one-click extra tools (Git, browser, GitHub and more).
- **@ mentions**: type @ to attach a file, a folder, an earlier chat, a memory, a web page or the Blender scene to a message.
- **Several models, one card**: use a fast chat and coding model plus a separate vision model for checking renders. Afiniel loads the right one for each step, keeps them loaded together when they fit, and swaps them when they don't, so smaller graphics cards don't run out of memory. A Low-VRAM mode keeps just one model loaded.
- **Models screen**: download recommended chat and coding models with one click, load, unload and remove them, and tune each model (context length, a GPU offload slider, sampling and more). **Auto-tune** measures a few settings and keeps the fastest.
- **Fast and clear**: real loading progress, a reply-time estimate, and LM Studio turns off when you close Afiniel so your graphics memory is free again.
- **Updates itself**: new versions download in the background and install with one click.

## Requirements

| | |
| --- | --- |
| **Operating system** | Windows 10 or 11, 64-bit |
| **LM Studio** | Free from [lmstudio.ai](https://lmstudio.ai). Afiniel can install and start it for you. |
| **An AI model** | Downloaded from inside Afiniel (Settings > Models). A vision model is best because it can also check images and renders. Recommended: **Qwen3-VL 30B A3B** for the best results, **Qwen3-VL 8B** for most PCs, **Qwen3-VL 4B** for small graphics cards and laptops. You can also add a coding model such as Qwen3 Coder next to it (Settings > Models > Model roles). |
| **Graphics card** | NVIDIA GPU recommended. 6 to 8 GB VRAM works with the small model, 12 GB is comfortable for 8B, 16 to 24 GB for the 30B model. It runs without a strong GPU too, just slower. |
| **Blender** (optional) | Only needed for 3D models. Blender 4.2 or newer, free from [blender.org](https://www.blender.org). Afiniel can install it for you. |
| **Disk space** | About 500 MB for Afiniel, plus 3 to 20 GB per AI model. |

## Install

1. Go to the [**latest release**](../../releases/latest) and download the **Setup .exe** under **Assets**. Or install it with winget: run `winget install Afiniel.AfinielAgent` in a terminal (available once Microsoft has approved the listing).
2. Run the installer.
3. **Windows SmartScreen** will probably say *"Windows protected your PC"*. That happens because the app isn't signed with a paid certificate, not because something is wrong. Click **More info**, then **Run anyway**.
4. Open **Afiniel Agent** from the Start menu or desktop.

## First start

1. **LM Studio**: if the LM Studio pill at the top is red, click it and choose **Start LM Studio for me** (or **Install LM Studio** if you don't have it).
2. **Pick a model**: open **Settings > Models**, choose one of the recommended models and press **Download**. When it's done, select it in the model picker at the top.
3. **Say hi.** Chat normally, or hand it a task: *"Compare the three best budget laptops for students"*, *"Clean up the notes in my Documents folder"* or *"Make a low-poly treasure chest with gold trim in Blender."*
4. **Blender**: the first time you ask for a 3D model, Afiniel opens Blender with its bridge add-on (or offers to install Blender). You can also click the Blender pill and choose **Open Blender for me**.

## Tips

- If replies are slow (the speed under a reply turns amber), the model doesn't fit your graphics card. Try a smaller model, press **Suggest settings for my GPU**, or run **Auto-tune** in Settings > Models.
- Using two models? **Settings > Models > Model roles** shows whether they fit on your card together. If they don't, Afiniel swaps them automatically, or you can turn on **Low-VRAM mode**.
- Each Blender step is one undo step: use **Revert last Blender step** under a render, or Ctrl+Z in Blender.
- Your chats, settings and renders are stored on your PC in `%APPDATA%\Afiniel Agent`.

## Updating

From version 1.0.10, Afiniel updates itself (the newest version is 1.1.0): when a new version is out it downloads in the background and shows **Restart to update**. You can also check in **Settings > Updates**. On older versions, download the newest installer from [Releases](../../releases) and run it. Your chats, memory and settings are kept.

---

<p align="center"><sub>Afiniel Agent is free to use. The source code is not published in this repository; it only hosts the README and the installer downloads.</sub></p>
