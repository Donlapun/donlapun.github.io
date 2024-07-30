---
name: Enhancing Optical Character Recognition (OCR) Capabilities for Historical Documents

tools: [Python, OCR, numpy, transformers, pandas, torch, Post-correction]
image: assets/pngs/sentence10_output.png
description: Digitize all the NASA Astrophysics Data System (ADS) historical text by using Optical Character Recognition (OCR) s
custom_js:
  - vega.min
  - vega-lite.min
  - vega-embed.min
  - justcharts
---

This project is a part of a NASA Astrophysics Data Analysis Program (ADAP) project aimed at creating several science-ready data products to help astronomers’ search the literature in new ways. It is also a part of Student Pushing Innovation (SPIN) Program under National Center for Supercomputing Applications (NCSA)

I trained post-correction model to correct the images from OCR output. Additionally, I conduct statistical analysis to evaluate the performances of the model to find new approaches to improve the accuracy.

Below is the example of the output of after passed to different post-correction models.

![OCR Output](/assets/pngs/sentence10_output.png)

Additionally, we investigated different methods to track **hallucinations** with several metrics such as Character Error Rate (CER) and Word Error Rate (CER), Jaccard Similarity, and Cosine Similarity.

The **future work** of this research will be focusing training the current model with new dataset and continue to explore other metrics to track hallucinations as well as training the model using Large Language Models (LLMs) for finding models that demonstrates optimal performance such as Astrollama, llama2, Gemini to improve the errors




