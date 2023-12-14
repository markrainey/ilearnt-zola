+++
title="How I learnt to run my own personal AI"
description="It is relatively easy to run your own personal instance of an AI similar to ChatGPT"
date=2023-12-14
authors = ["Mark Rainey"]
[taxonomies]
categories=["ai","howto"]
tags=[]
+++

By now most people have tried or at least heard of ChatGPT. It is now relatively easy to run your own AI instance on your own machine.

<!-- more -->

One free tool that makes this simpler is LM Studio. It is a desktop application that you can run locally on your machine. You download and then select whichever LLM (large language model) you want to use to run it. Don't worry, LLM basically means the brains and knowledge you want to use to ask questions.

To install it, go to the LM Studio [website](lmstudio.ai) and download the version for the operating system you use (MacOS, Windows or Linux) and install it.

Once it is installed, run the application.

<img src="/posts/LmStudio1.png" title="Lm Studio1" class="mid-image"></img>

The first thing you will need to do is download the LLM. There is a daunting array of models and it is not easy to decide which. I did a little research and I have downloaded two models to play with:

zephyr beta (q4_k_s)
orca 2 (q5_k_m)

You can search for a specific model or scroll through the list. To download one, select the instance you want and click the "Download" button next to it. It might take a while to download as they tend to be between 4-8Gb.

Once loaded you will want to try it out. Click on the chat icon (3rd one down) on the left hand side. At the top there is a dropdown to select the model to use - this will load it into memory. 

<img src="/posts/LmStudio2.png" title="Lm Studio2" class="mid-image"></img>

Once it is loaded you can start a new chat. A text box will appear where you can type your prompt and answers will appear below it.

<img src="/posts/LmStudio3.png" title="Lm Studio3" class="mid-image"></img>

You are now free to play.

You can also run it as a local web server so you can query it using CURL or from an API.

<img src="/posts/LmStudio4.png" title="Lm Studio4" class="mid-image"></img>

Note, sometimes it will occasionally  stop generating responses. Usually this can be solved by reloading the model from the dropdown or worst case restarting the application. Your previously downloaded models will still be available and don't need to be downloaded again - you just need to select the model before chatting as before.

__Links__

[LM Studio](https://lmstudio.ai/)
