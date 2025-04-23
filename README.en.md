# redstar upscaler
Powerful video upscaling tool using FFmpeg, Real-ESRGAN, Flowframes - now supports **multi-language UI**!

🌐 Language:
[English](README.en.md) | [한국어](README.md) | [日本語](README.ja.md) | [中文](README.zh.md) |
[Français](README.fr.md) | [Deutsch](README.de.md) | [Español](README.es.md) | [Português](README.pt.md) |
[Русский](README.ru.md) | [Italiano](README.it.md) | [Tiếng Việt](README.vi.md) | [Bahasa Indonesia](README.id.md) |
[ภาษาไทย](README.th.md) | [العربية](README.ar.md)

<p align="center">
  <img src="https://github.com/user-attachments/assets/632c3a83-5416-46c3-8d38-0e1bf153b633" height="250"/>
</p>

<p align="center">
  <strong>Video upscaling tool based on fmpeg, realesrgan, flowframes</strong><br>
  <em>Modern GUI based, preset settings, support for multi-file processing</em>
</p>

---.

Download: [Release](https://github.com/redstar-programmer/upscaler/releases/)

## ✨ Please support redstar' upscaler

Do you like this project or want to support its development?
Help us build better features and stable updates with a small donation!

- <img src="https://img.shields.io/badge/Donate-PayPal-blue.svg?logo=paypal" height="20"/><br>**PayPal** : [https://paypal.me/redstarprogrammer?country.x=KR&locale.x=ko_KR](https://paypal.me/redstarprogrammer?country.x=KR&locale.x=ko_KR)
- <img src="https://img.shields.io/badge/Sponsor-GitHub%20Sponsors-ff69b4?logo=githubsponsors" height="20"/><br>**GitHub Sponsors** : [https://github.com/sponsors/redstar-programmer](https://github.com/sponsors/redstar-programmer)


> 💡 Your sponsorship of server costs, development time, and a cup of coffee goes a long way. Thank you!

## Table of Contents

- [👋 Introduction] (#Introduction)
- [💾 Installation and Preparation](#Installation-and-Preparation)
- [🔧 Main Features](#Main-Features)
- [🚀 How to use (Quick Start)](#How-to-use-quick-start)
- [⚙️ Detailed Feature Description](#detailed-feature-description)
- [🙏 Acknowledgments](#Acknowledgments)
- [📜 History](#history)

## 👋 Introduction
**redstar upscaler is a Python-based GUI tool to automatically upscale videos to higher resolutions using `ffmpeg`, `Real-ESRGAN`, and `Flowframes`.

- Extract video frames → upscale → merge videos in one step
- Supports various realesrgan models
- Optional interpolation via Flowframes
- Automatic extraction and processing of audio codecs
- Work on source location or specified path

> ⚠️ Developed and tested in a Windows environment.

Below is a simple usage demo:<br>
![미디어1](https://github.com/user-attachments/assets/ba601a08-6749-45fd-ae21-f1a2a52987f6)

## 💾 Installation and Preparation

1. install and locate the following external tools (note that the distribution file includes ffmpeg, Real-ESRGAN, and Flowframes installers (see Programs folder in the path))
   - [ffmpeg](https://www.ffmpeg.org/download.html)
   - [Real-ESRGAN](https://github.com/xinntao/Real-ESRGAN/releases)
   - [Flowframes](https://github.com/n00mkrad/flowframes) *(optional)
2. unzip and run readstar's upscaler.exe
3. in the case of Flowframes, the models loaded may be different depending on your environment, so be sure to run Flowframes and make sure that the Interpolation AI and AI Model in the Interpolation tab match the version of redstar upscaler's resources/flowframes_models.ini. <br>Comment out the models that are not loaded by marking them with # and make sure that the order of models in redstar upscaler's settings window matches the order of models in <br>Flowframes.

## 🔧 Main Features

![Image](https://github.com/user-attachments/assets/072af636-e967-4e4b-b194-33b96f580780)
- ✅ Multiple video selection and sequential operation
- ✅ Add drag/drop video
- ✅ Main program availability and direct selection
- Disk saving mode
- ✅ Multilingual support (15 languages)
<br><br>
![Image](https://github.com/user-attachments/assets/23dd7e8a-0e01-409f-b162-a9512fda09fc)
- Save and automatically apply presets
- Automatic audio codec detection and bitrate setting
- Automatic detection and selection of realesrgan models
- ✅ Detailed settings for FFMPEG, real-ESRGAN and Flowframes
- ✅ Change option settings according to Flowframes version<br>(Version can be changed by specifying the path to the version in flowframes on the main page)
<br><br>
![Image](https://github.com/user-attachments/assets/ab7d9410-1fb4-450b-92d5-56a6d583a64c)
- ✅ Check the upscale execution command (you can copy and execute it separately on CMD)
<br><br>
![Image](https://github.com/user-attachments/assets/4898904a-bb23-4dba-997d-23ca744fed93)
- Monitor the overall progress of the upscale job
- ✅ Check upscale logging (log files are created by date in the log folder in the live folder)
- Automatically organize deliverables after job completion (prefixed with [REDSTAR])
- ✅ Configurable action after task completion<br>( Do nothing / Close program / Sleep mode / Hibernate mode / Close window)
<br><br>
## 🚀 How to use (Quick Start)

1. add video files (MP4, MKV, AVI, MOV, FLV, WMV, MPG, WEBM, 3GP, OGV supported)
2. specify the working location or check "Use original file path"
3. click "Settings" button on the added video
4. ffmpeg, realESRGAN, Flowframes detailed settings
5. click Batch apply to all files / Apply to selected files only
6. click "Confirm" button
7. check the commands to be executed and click the Start Task button

> ✨ The result of the job will be two files: upscaled video and frame interpolated video in the selected folder.
> ✨ The completed files will be saved with a filename prefixed with [REDSTAR].
---]

## ⚙️ Detailed Feature Description

| Item | Description |
|------|------|
| **Set working path** | Provide default path or "Use original file path" option |
| **Video format support** | Most formats supported, including MP4, MKV, AVI, MOV, FLV, WMV, MPG, WEBM, 3GP, OGV, etc.
| **Upscale models** | Automatically detects realesr-animevideov3, realesr-general, 4xplus, etc.
| **Audio processing** | Support for encoding various formats such as `aac`, `mp3`, `flac`, etc.
| **Flowframes integration** | Interpolation (FPS ×2, ×4, ×8) can be set
| **Disk Saving Mode** | Automatic deletion of intermediate images

## 🙏 Acknowledgments

- realesrgan by [xinntao](https://github.com/xinntao/Real-ESRGAN)
- flowframes by [n00mkrad](https://github.com/n00mkrad/flowframes)
- If you would like to contribute to this project or suggest a feature, please leave a comment on [Issues](https://github.com/redstar-javscraper/redstar_upscaler/issues).

# 📜 History

v 1.1.0
 > 1. menu organization (open file, close file, log settings, language settings)
 > 2. added multi-language settings (available languages: Korean, English, 日本語, 中文, Français, Deutsch, Español, Português, Русский, Tiếng Việt, Bahasa Indonesia, ไทย, Italiano, العربية)
 > 3. Changed the message and some code for adding language settings
 > 4. some UI configuration changes
 > 5. ffmpeg, real-ESRGAN, Flowframes version information (main screen)
 > 6. Support Flowframes 1.41.0 version (currently only 1.40.0, 1.36.0 versions are available due to cmd command issue in 1.41.0 version)
 > 7. Fixed an issue where AI Models items were displayed in lowercase letters
 > 8. Added FFMPEG options (Pixel, video codec) - options are displayed according to the user's PC
 > 9. Enhanced CUDA check for user's PC - check availability and GPU type (main screen)

v 1.0.0
 > 1. Full code rewrite
 > 2. UI changes
 > 3. Increased the range of video/audio that can be processed
 > 4. added disk saving mode
 > 5. Distribution including major programs

v 0.1.92
 > 1. Fixed an issue that caused interpolation to fail due to duplicate entries in the AI model combo box when changing the Flowframes path.
 > 2. Added a check code for the selection status of the combo box when interpolating.

v 0.1.91
 > 1. Added some combobox refresh functions related to Flowframes
 > 2. Adjusted some distribution files

v 0.1.9
 > 1. Apply Flowframes model changes
 > 2. implemented Flowframes 1.36.0 new model, 1.40.0 model
 > 3. Flowframes command line failure no longer occurs
 > 4. Files can now be added by dragging/dropping
 > 5. Fixed Flowframes settings not being applied

v 0.1.8
 > 1. Fixed new version check error when checking version
 > 2. if flowframes is installed in the default path (ex. C:\Users\Administrator\AppData\Local\Flowframes\), set the path as default before starting.
 > 3. When adding multiple file selections, the application crashes due to an error.
 > 4. Fixed an error when starting the task after adding multiple files

v 0.1.7
 > 1. Program size can be changed
 > 2. Fixed an error when working with files without voice
 > 3. changed the whole UI configuration (reorganized to fit the size change)

v 0.1.6
 > 1. Fixed issue with different font sizes depending on screen resolution
 > 2. Fixed an issue where the program title does not show the version information as a new version
 > 3. fixed an issue where the config.ini file was saved in a different path
 > 4. When changing the realesrgan upscaling multiplier, the upscaling model combo box is also changed.
 > 5. added update check function
 > 6. fixed some logic
 > 7. changed the color of resolution and fps tables
 > 8. Allow user to modify resolution (must be entered in 1024x768)

v 0.1.5
 > 1. Fixed issue where AI model is not automatically changed when selecting FLOWFRAMES interpolation AI
 > 2. fixed an issue where flowframes interpolation was not interpolated as per the selected option
 > 3. Added "FPS calculation method" combo box to prevent incorrect FPS calculation for some videos.
        -> r_frame_rate / avg_frame_rate, default is r_frame_rate
 > 4. Show video information fetching progress when selecting a video file
 > 5. change to default to open last selected folder when selecting a file again after opening a file

v 0.1.4
 > 1. changed the way to read config.ini file
 > 2. changed the way to fetch video information from Python AV to ffmpeg
 > 3. added window closing function when task ends
 > 4. Show full filename as tooltip on mouseover in task list
 > 5. show resolution(before) / resolution(after) / FPS(before) / FPS(after) for each file in task list
 > 6. remove FPS input box (due to above labeling for each file)
 > 7. Remove Output FPS Estimated Size (due to the above file-specific notation)
 > 8. display progress as two progress bars for all files/jobs

v 0.1.3
 > 1. Fixed file FPS calculation error where some FPS information was wrong when loading files

v 0.1.2
 > 1. UI configuration changes
 > 2. internal logic changes
 > 3. fixed the problem that realesrgan model does not run when selecting two of the following models
 > 4. changed the way to use realesrgan models
 > -> Copy the new model file (*.param) to the models folder in the realesrgan installation folder and you can use it.
 > 5. display width, height information and estimated upscale size of the last file of the target image to work with
 > 6. write code to migrate config.ini file
 > 7. change FFMPEG decomposition image AAC -> FLAC
 > 8. other bug fixes

v 0.1.1
 > 1. First time writing, video upscaling program with ffmepg, realesrgan and flowframes