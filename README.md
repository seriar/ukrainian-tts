---
title: "Ukrainian TTS"
emoji: 🐸
colorFrom: green
colorTo: green
sdk: gradio
app_file: app.py
pinned: false
---

# Ukrainian TTS 📢🤖
Ukrainian TTS (text-to-speech) using Coqui TTS.

Trained on [M-AILABS Ukrainian dataset](https://www.caito.de/2019/01/the-m-ailabs-speech-dataset/).  

# Example

https://user-images.githubusercontent.com/5759207/139459556-35aa077b-0425-421f-a8d3-4c503315008d.mp4

# How to use :
1. `pip install -r requirements.txt`.
2. Download model from "Releases" tab.
3. Launch as one-time command:  
```
tts --text "Text for TTS" \
    --model_path path/to/model.pth.tar \
    --config_path path/to/config.json \
    --out_path folder/to/save/output.wav
```
or alternatively launch web server using:
```
tts-server --model_path path/to/model.pth.tar \
    --config_path path/to/config.json
```

# How to train:
1. Refer to ["Nervous beginner guide"](https://tts.readthedocs.io/en/latest/tutorial_for_nervous_beginners.html) in Coqui TTS docs.
2. Instead of provided `config.json` use one from this repo.


# Attribution
Code for `app.py` taken from https://huggingface.co/spaces/julien-c/coqui