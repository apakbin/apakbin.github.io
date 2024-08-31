---
layout: home
title: Arash Pakbin
---

# Howdy!

<div style="text-align: justify;margin-bottom: 10px;"> My name is Arash Pakbin. I am a Ph.D. candidate in the Computer Science and Engineering Department at Texas A&M University, working under the mentorship of <a href="https://engineering.tamu.edu/cse/profiles/mortazavi-bobak.html">Dr. Bobak J. Mortazavi</a> and <a href="https://goizueta.emory.edu/faculty/profiles/donald-lee">Dr. Donald K.K. Lee</a>. I previously interned at Tesla Autopilot, where I gained valuable industry experience. My dissertation, "Interpretable Functional Data Boosting in Survival Analysis," introduces a boosting algorithm for hazard estimation. For more details on this project, visit its <a href="https://github.com/BoXHED/BoXHED2.0">Github page</a>.</div>


<div style="text-align: justify;margin-bottom: 10px;"> In recent projects, I developed a multimodal real-time risk monitoring system for ICU settings by leveraging a language model. This system integrates time-series data with clinical notes to enhance real-time risk assessment capabilities. Additionally, I am exploring techniques for summarizing clinical texts using language models and adapting them for training smaller models with constrained context lengths.</div>

<div style="text-align: justify;margin-bottom: 10px;"> I am currently seeking my first industry position, where I can apply my expertise in these areas. Feel free to reach out—email is my preferred method of communication.</div>


***

<h2 style="margin-bottom: 10px;">Sample Code</h2>

<p style="margin-bottom: 10px;">Here are a few examples of my work:</p>

<ul>
  <li style="text-align: justify;margin-bottom: 10px;">In <a href="https://github.com/BoXHED/BoXHED2.0-source-code/tree/master/packages/boxhed_prep/boxhed_prep">this project</a>, I developed a data preprocessing pipeline that extends <span style="font-family: Courier New;">Python</span> with <span style="font-family: Courier New;">C++</span>. The pipeline generates data in <span style="font-family: Courier New;">Python</span> and processes it in <span style="font-family: Courier New;">C++</span> for scalability, utilizing <span style="font-family: Courier New;">numpy</span> and <span style="font-family: Courier New;">ctypes</span> in <span style="font-family: Courier New;">Python</span>, and <span style="font-family: Courier New;">OpenMP</span> in <span style="font-family: Courier New;">C++</span>.</li>
  <li style="text-align: justify;margin-bottom: 10px;">In <a href="https://github.com/apakbin/UNET-Implementation">this project</a>, I implemented a <span style="font-family: Courier New;">U-Net</span> architecture using <span style="font-family: Courier New;">PyTorch</span>. This design features two types of convolution layers: a standard <span style="font-family: Courier New;">conv2d</span> layer and an optimized convolution layer that reduces parameters by decreasing kernel size while maintaining the receptive field by shifting channels along the time dimension.
</li>
</ul>
***

<h2 style="margin-bottom: 10px;">Projects</h2>

Here is a selection of my key projects, along with an overview of each.

<h3 style="margin-bottom: 0px;">Text Summarization for Multimodal Pretraining of Medical Data</h3>
<h6 style="margin-bottom: 5px;">Aug 2024 – Present</h6>
<ul>
  <li style="text-align: justify;margin-bottom: 5px;">ICU clinical notes can be lengthy, requiring large context lengths for language models to capture the full content.</li>
  <li style="text-align: justify;margin-bottom: 5px;">Training language models with large context lengths is computationally prohibitive.</li>
  <li style="text-align: justify;margin-bottom: 5px;">We use a <span style="font-family: Courier New;">Llama3-8B</span> model for summarizing notes through in-context learning, fitting them into a <span style="font-family: Courier New;">BERT</span> model with a 512 context length.</li>
  <li style="text-align: justify;margin-bottom: 5px;">More details coming soon!</li>
</ul>

<hr style="width:50%; margin-left:25% !important; margin-right:25% !important;" />

<h3 style="margin-bottom: 0px;">Real-time, Multimodal Invasive Ventilation Risk Monitoring using Language Models and BoXHED</h3>
<h6 style="margin-bottom: 5px;">Jan 2024 -- Aug 2024</h6>
<div style="text-align: center; margin-bottom: 15px;">
        <img src="/assets/figs/mmb.png" width="600" height="auto" class="center">
</div>
<ul>
  <li style="text-align: justify;margin-bottom: 5px;">Conventional invasive ventilation monitoring in ICUs often ignores clinical notes and relies solely on time-series data.</li>
  <li style="text-align: justify;margin-bottom: 5px;">Achieved <span style="font-family: Courier New;">AUROC</span> of 0.86 and <span style="font-family: Courier New;">AUCPR</span> of 0.35 by combining clinical text data with time-series data.</li>
  <li style="text-align: justify;margin-bottom: 5px;">Used a <span style="font-family: Courier New;">T5</span> language model to extract numerical representations from clinical notes.</li>
  <li style="text-align: justify;margin-bottom: 5px;">Reduced inference latency by 8 times with <span style="font-family: Courier New;">PyTorch</span> multiprocessing for multi-GPU inference.</li>
</ul>

<hr style="width:50%; margin-left:25% !important; margin-right:25% !important;" />

<h3 style="margin-bottom: 0px;">Scalable Boosting of Dynamic Survival Analysis</h3>
<h6 style="margin-bottom: 5px;">Jan 2020 -- Dec 2023</h6>
<div style="text-align: center; margin-bottom: 15px;">
  <img src="/assets/figs/hazard.png" width="500" height="auto" class="center" />
  <figcaption>Estimation of hazard values as a function of time and a covariate.</figcaption>
</div>
<ul>
  <li style="text-align: justify;margin-bottom: 5px;">Created <span style="font-family: Courier New;"><a href="https://github.com/BoXHED/BoXHED2.0">BoXHED</a></span>, a <span style="font-family: Courier New;">Python</span> package for nonparametric hazard estimation.</li>
  <li style="text-align: justify;margin-bottom: 5px;">Achieved 35%+ error reduction and 900x speedup with GPU and multicore CPU support.</li>
  <li style="text-align: justify;margin-bottom: 5px;">Published <span style="font-family: Courier New;">BoXHED1.0</span> at <a href="http://proceedings.mlr.press/v119/wang20o/wang20o.pdf">ICML</a> and <span style="font-family: Courier New;">BoXHED2.0</span> in <strong>Journal of Statistical Software</strong> (preprint on <a href="https://arxiv.org/abs/2103.12591">arXiv</a>).</li>
  <li style="text-align: justify;margin-bottom: 5px;">Integrated code with the <span style="font-family: Courier New;">XGBoost</span> library codebase and made available on <span style="font-family: Courier New;">PyPI</span>.</li>
  <li style="text-align: justify;margin-bottom: 5px;">Open-source code is accessible on <a href="https://github.com/BoXHED/BoXHED2.0-source-code">Github</a>.</li>
</ul>

***

<h2 style="margin-bottom: 10px;">Skills</h2>

<p style="margin-bottom: 10px;">These are the areas where I excel:</p>

| **Languages**         | <span style="font-family: Courier New;">Python</span> / <span style="font-family: Courier New;">C++</span> / <span style="font-family: Courier New;">CUDA C</span> / <span style="font-family: Courier New;">R</span> |
| **Tools (<span style="font-family: Courier New;">Python</span>)**    | <span style="font-family: Courier New;">PyTorch</span> / <span style="font-family: Courier New;">Transformers</span> / <span style="font-family: Courier New;">Hugging Face</span> / <span style="font-family: Courier New;">Pandas</span> / <span style="font-family: Courier New;">Weights & Biases</span> / <span style="font-family: Courier New;">DeepSpeed</span> / <span style="font-family: Courier New;">NumPy</span> |
| **Machine Learning**  | <span style="font-family: Courier New;">Transformers</span> / <span style="font-family: Courier New;">Generative AI</span> / <span style="font-family: Courier New;">Language Models</span> / <span style="font-family: Courier New;">NLP</span> / <span style="font-family: Courier New;">Distributed Training</span> / <span style="font-family: Courier New;">Model Transparency</span> / <span style="font-family: Courier New;">Boosting</span> |
| **General**           | <span style="font-family: Courier New;">Linear Algebra</span> / <span style="font-family: Courier New;">Time Series Analysis</span> / <span style="font-family: Courier New;">Statistical Modeling</span> / <span style="font-family: Courier New;">AWS</span> |
