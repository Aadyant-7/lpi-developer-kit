# Track A

Github Repo Link - https://github.com/PriyanshuBHardwaj20/lpi-agent

### What I did,step by step for L3

1) Set up a virtual environment to manage dependencies like requests.

2) Integrated the LPI Developer Kit's Node.js server into a Python script using the subprocess module to establish a JSON-RPC connection over stdio.

3) Programmed the agent to query multiple LPI tools, specifically smile_overview and smile_phase_detail , to gather grounded methodology data.

4) Connected the agent to a local LLM via Ollama (Qwen 2.5:1.5b) to perform a Gap Analysis that compares a user's project state with the SMILE framework.

5) Engineered a system prompt that forces the LLM to provide citations for every claim, ensuring the user can trace the answer back to the specific LPI tool used.

6) Implemented a streaming response logic to provide real time feedback and prevent timeouts during long analysis generations.

### Problems I Hit & How I Solved Them For L3

I initially couldn't activate my virtual environment in PowerShell due to execution policies. I solved this by switching to the Command Prompt, which bypassed the script restriction. The Qwen 3.5 model was too heavy for my Laptop, causing the script to hang or timeout. I solved this by switching to the Qwen 2.5:1.5b model, which is much faster.

### What I Learned That I Didn't Know Before L3

I learned how to use MCP to bridge different programming environments to create a unified AI system.

# Track D

Github Repo Link - https://github.com/PriyanshuBHardwaj20/digital-twin

### What I did,step by step for L3

1) created a new unity project with standard 3D URP template.

2) then created a 3d hospital room for digital twin concept using primitive 3D shapes.

3) inside the room I created Bed, Patient and Patient Monitor game_objects using primitive 3D shapes.

4) Using Unity's UI system I created a screen for Patient Monitor and Patient Vitals UI which has sliders for changing different patient vitals for simulating Patient health.

5) Finally i created a C# script for changing the Patient's colour based on its Vitals. 

### Problems I Hit & How I Solved Them For L3

The main problem I faced was to decide what digital twin concept I should choose and how it would look like in Unity, to solve this I googled existing digital twin concepts made in Unity, and I found "Introduction to Digital Twins with Unity"
on Unity learn website which helped me a lot to decide the digital twin concept. I hardly faced any technical challenge as I have worked with Unity for a long time. 

### What I Learned That I Didn't Know Before L3

I learned a lot about digital twins and how I can implement them using Unity.


