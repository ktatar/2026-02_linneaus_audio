---
marp: true
theme: my_theme
math: katex
paginate: true
---

<!-- footer: <small><i style="font-size: 8pt;font-weight:500;color:black">AI in Computational Arts, Music, and Games </small></i> <p> ![width:350](chalmers-gu.png)</p> -->
<!-- _color: black -->

# Sound, Machine Learning, and Deep Generative Models: A Practical Introduction

![bg opacity:10% ](img/wave-stft-onset.png)

---

![align-right width:700](img/wave-stft-onset.png)

## Basics of Sound concepts

- Waveform: dynamics, transients, envelopes
- Frequency: pitch, overtones, timbre components
- Time–frequency transforms: spectrograms, mel spectrograms
- Energy and dynamics over time (envelope, loudness curves etc.)

<small>McFee, Brian, Colin Raffel, Dawen Liang, Daniel PW Ellis, Matt McVicar, Eric Battenberg, and Oriol Nieto. "librosa: Audio and music signal analysis in python." In Proceedings of the 14th python in science conference, pp. 18-25. 2015. </small>


---

### Waveforms and Their Features

- General Introduction:
https://www.audiolabs-erlangen.de/resources/MIR/FMP/C1/C1S3_Waveform.html
-Phase: https://images.contentful.com/piwi0eufbb2g/5HdnEvKEB7URTVKDH4iIhf/4ee0fc97b8ac2fe046c195bfc5484228/0_QFVha2lCgyhKjhuO.gif
- Dynamics and Loudness
https://www.audiolabs-erlangen.de/resources/MIR/FMP/C1/C1S3_Dynamics.html
- Envelope Calculation
https://www.audiolabs-erlangen.de/resources/MIR/FMP/C1/C1S3_Timbre.html
- Onset detection: 
https://www.audiolabs-erlangen.de/resources/MIR/FMP/C6/C6S1_OnsetDetection.html

---

## Timbre and its features

### FFT based
  - Fast Fourier Transform: https://pythonnumericalmethods.studentorg.berkeley.edu/notebooks/chapter24.04-FFT-in-Python.html
  - Short-time Fourier Transform: https://www.audiolabs-erlangen.de/resources/MIR/FMP/C2/C2_STFT-Basic.html
  - Time vs Frequency Resolution in FFTs: https://support.ircam.fr/docs/AudioSculpt/3.0/co/Window%20Size.html
  - Mel-frequency Cepstral Coefficients
    - Compute pipeline: https://www.researchgate.net/publication/257365356/figure/fig2/AS:297528441491462@1447947716655/Calculation-process-of-MFCC-coefficients.png
    - Example: https://librosa.org/doc/latest/generated/librosa.feature.mfcc.html

---

### Wavelet based Timbre Features

- Constant-Q Transform:
    https://librosa.org/doc/latest/generated/librosa.cqt.html
- Variable-Q Transform:
  https://librosa.org/doc/latest/generated/librosa.vqt.html


<small> [1] Schorkhuber C, Klapuri A (2010) Constant-Q Transform Toolbox
For Music Processing. In: Proceedings of the 7th Sound and Music Computing Conference (SMC 2010), p. 8. Barcelona, Spain 
</small>

---

# Music Specific Features
  Music specific
- Pitch:
  https://docs.pytorch.org/audio/stable/tutorials/audio_feature_extractions_tutorial.html#sphx-glr-tutorials-audio-feature-extractions-tutorial-py 
- Multipitch (chroma):
  - https://librosa.org/doc/latest/feature.html#spectral-features

- Beat detection: 
  - https://librosa.org/doc/latest/generated/librosa.beat.beat_track.html
---

## Machine Learning for Sound and Music Computing

---

### Importance of Feature Representations in Machine Learning

![align-center width:600](img/features-matters.png)

<small>I. Goodfellow, Y. Bengio, and A. Courville, Deep Learning. MIT Press, 2016.</small>

--- 

### Dimensionalty reduction

- Principle Component Analysis
https://musicinformationretrieval.com/content/10_decomposition/pca.html

- UMAP: Uniform Manifold Approximation and Projection: https://www.kaggle.com/code/adampq/umap-projections-little-shop-of-horrors-audio
  
- T-distributed stochastic neighbor embedding: https://ml4a.github.io/guides/AudioTSNEViewer/
  - Notes on t-SNE: https://dash.gallery/dash-tsne/
---

### Machine Learning 

- Supervised Learning 
- Unsupervised Learning

Detailed resources: https://www.ibm.com/think/machine-learning#605511093

---

### Supervised Learning - Classification

![align-center width:600](img/mnist-classification.png)


<small>Image source: https://medium.com/data-science/image-classification-in-10-minutes-with-mnist-dataset-54c35b77a38d 
</small>

---

### Supervised Learning - Audio Classification

Mediapipe: https://ai.google.dev/edge/mediapipe/solutions/audio/audio_classifier

---

### Supervised Learning - Regression

![align-center width:500](img/linear-regression.png)

<small>Image source: https://python.plainenglish.io/understanding-multiple-linear-regression-in-machine-learning-58e981ce7747
</small>

---

### Unsupervised Learning - Clustering

---

###

---

### Deep Learning


--- 

### Deep Learning - Fun Visualizations

- https://adamharley.com/nn_vis/
- https://www.bulovic.at/cnn/

---

Distances

  For signals and features
    Eucledian 
    Cosine 
    Frechet Audio Distance
  For distributions
    KL-Divergence


---
DL based feature representations

  Deep Embeddings
  Autoencoders
  CLAP 

---

ML things one could do


---

---
# What is TRA 385?

This is a list:

- item 1
- item 2
- item 3

---

# This is a table 

| Activities  |  |  | | |
|:---|---|---|---|---|
| **Lectures** | Introduction to Art and Technology | Introduction to AI and ML | Creativity, Group work, and Tools for Innovation |
| **Tutorials** | Creative Coding with Sound (PureData) | Multimedia Design with TouchDesigner | Deep Learning for Multimedia | Interactive ML with Physical Computing |
| **Project** |Project Proposal| Design Iterations | Final Prototype | Reflections |

---
<!-- _class: no_border -->

# This is the same table without borders

| Activities  |  |  | | |
|:---|---|---|---|---|
| **Lectures** | Introduction to Art and Technology | Introduction to AI and ML | Creativity, Group work, and Tools for Innovation |
| **Tutorials** | Creative Coding with Sound (PureData) | Multimedia Design with TouchDesigner | Deep Learning for Multimedia | Interactive ML with Physical Computing |
| **Project** |Project Proposal| Design Iterations | Final Prototype | Reflections |

See how *Activities* are not bold now. That is because th class is updated in section.no_border class in my_theme.css  

---
<!-- _class: columns -->

<div>

## Two column slide

Originally solution from <https://github.com/orgs/marp-team/discussions/192#discussioncomment-1516155>

</div>
<div>

## Can't believe this works. YOLO

If you are brave for more sections, here is an online tool for css grids: https://grid.layoutit.com/

</div>

---

# Image on the left

![bg left](fuse.jpg)

---

# AND Image on the right

![bg right](fuse.jpg)

---

# Image aligned on the left

![align-left width:400](fuse.jpg)

---

# Image aligned on the right

![align-right width:400](fuse.jpg)

---

# Image aligned at the center

![align-center width:400](fuse.jpg)

---

# Local videos are possible 

<video controls src="pb-ars.mp4" width="800"></video>

---

# Online videos as well 

<iframe width="560" height="315" src="https://www.youtube.com/embed/nx2Nj3I7NyU?si=5D-PemuLUUt3qepd&amp;controls=0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

This should work only when the presentation is hosted online. Youtube does not allow local hosts apparently.

---

# Fancy image options

![bg left:40% width:500px](fuse.jpg "Fuse it up" )

`<br/>` command works for creating empty spaces [2].

<br/>

<small>[1] this is a smaller text. Great for citations. 

[2] https://marpit.marp.app/image-syntax
</small>

---

# Inline HTML commands works 

<p style="text-align: center;font-size:64px;color:red;"> Text can be <span style="font-size:48px;color:black;">changed</span> for example </p>

---

# <!--fit-->BIG TEXT

---

# How to export to github pages? 

- Copy this template
- Setup github pages to deploy from a branch. Choose main branch. 
  - There is no workflow, so that what you see local is what you get online as a static html. 
- Once you are done with your presentation, render it to html locally.
  - On VS Code, you can just use the marp icon on the top right. 
  - Make sure the file saved is index.html.  
- Commit changes to the remote repo.
- Done! Page should be online at [user-name].github.io/[repo-name] after a few minutes.

---

# Latex Math friendly

## Inline math

Render inline math such as $ax^2+bc+c$ [1].

## Math block

$$ I_{xx}=\int\int_Ry^2f(x,y)\cdot{}dydx $$

$$
f(x) =
  \int_{-\infty}^\infty
  \hat f(\xi)\,e^{2 \pi i \xi x}
  \,d\xi
$$

</br>

<small>[1] More details: https://github.com/marp-team/marp/blob/main/website/docs/guide/math-typesetting.md </small>

---

# Videos need to be formatted for web

You can use ffmpeg locally for this.

`ffmpeg -i input.mp4 -c:v libvpx-vp9 -crf 30 -b:v 0 output.webm` 

note: tested and works

<small>[1] Source: https://jshakespeare.com/encoding-browser-friendly-video-files-with-ffmpeg/ </small>

---

# FFMPEG continued: another solution

fast and efficient h264 for the web :

`ffmpeg -i in.mp4 -c:v libx264 -profile:v high -preset slow -crf 24 -c:a aac -b:a 96k -movflags +faststart out.mp4`

More efficient but slower with VP9/webm

`ffmpeg -i in.mp4 -c:v libvpx-vp9 -crf 33 -b:v 0 -c:a libopus -vbr on -b:a 64k out.webm`

<small>[1] https://www.reddit.com/r/ffmpeg/comments/8kxjhz/encoding_video_for_my_website/ </small>

---

# FFMPEG continued

I haven't tried this solution yet.

WebM:

`ffmpeg -i my-original-video.wmv -f webm -vcodec libvpx-vp9 -vb 1024k my-new-video.webm`

MP4: 

`ffmpeg -i my-original-video.wmv -vcodec libx264 -f mp4 -vb 1024k -preset slow my-new-video.mp4`

<small>[1] Source: https://jshakespeare.com/encoding-browser-friendly-video-files-with-ffmpeg/ </small>