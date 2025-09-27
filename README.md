# 🧪 Vison Labeling Agent

## 🧠 Overview

- Traditional object-detection has been a closed domain problem where ML models can only detect predefined set of objects (closed vocabulary) that the models were explictly trained on.

- These models can not detect arbitary objects without training on new dataset
- However, the unfolding of the multi-models have enabled us to open-vocabulary object detection without being explicitly trained on in-domain data:
- There're two types of multi-models can be seen in the production environments:
    1. Vision Language Models (VLMs): Models which can handle both text and image data
        - Florence-2, Llama-3.2-vision, Gemini-2.5, GPT-4o, Moonderam-3.0
    2. Omni Models: Models which can handle multiple data types - text, image, video (images with time dimension), audio

- Since novel LLMs/VLMs can be configured in an agentic way (observe, think and act), detecting arbitary objects in an image or a video becomes a ease of task without explicit training on new domains
    - However, if your domain data is completely different from what the VLM has been trained on, in that case you still need a fine-tuning step to get better results
    - Otherwise, typical off shelf models like Gemini, GPT4o, Moondream would work

### Overview of Agentic Object Detection

Agentic Object Detection goes beyond traditional detection by:
- Understanding **user intent** from natural language input
- Using **reasoning agents** to guide and refine detection
- Leveraging **Open-vocabulary models** to detect a wide range of objects:
    - This could be another VLM (Florence-2, Moondream-3, etc)

