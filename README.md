# Video Restoration with Pretrained DL Models

An end-to-end video restoration project by using the-state-of-art deep neural network models. Only pretrained and open-source repositories on Github were used to produce the end result, without doing any training task.

In this repository, video restoration methods are reviewed and implemented by using cited repositories and papers with the demonstration of the results. <a href="https://www.youtube.com/watch?v=5yeNO-l7OLc">Sample video</a> was used for the restoration example.

## Results

- <a href="https://www.youtube.com/watch?v=UtgXiHRS_nc">Final vs Original</a>
- <a href="https://www.youtube.com/watch?v=qqaCTEEdVYA">Final Postprocessing (4K + 50FPS) </a>
- <a href="https://www.youtube.com/watch?v=qjg2-W09Yp0">Fully Automatic Video Colorization with Self-Regularization and Diversity</a>

### Environments

- Google Colab
- Anaconda
- Local:

&nbsp;&nbsp; **OS**: Windows 10 Home 64-bit

&nbsp;&nbsp; **GPU**: GeForce GTX 1060 Max-Q 

&nbsp;&nbsp; **CPU**: Intel i7-7700HQ

&nbsp;&nbsp; **RAM**: 16GB

## Sample Video Properties

- **Length** : 00:01:49
- **Width** : 640
- **Height** : 480
- **Frame per second**: 25
- **Number of frames**: 2726
- **Format** : .mp4

## Resources
### Super Resolution:

&nbsp;&nbsp; EDSR, WDSR and SRGAN for single image super-resolution that requires the Keras Tensorflow backend.

- <a href="https://github.com/krasserm/super-resolution/tree/previous" target="_blank">Github</a>

### Video frame interpolation

&nbsp;&nbsp; Depth-Aware Video Frame Interpolation (CVPR 2019)
- <a href="https://github.com/baowenbo/DAIN" target="_blank">Github</a> 

- <a href="https://sites.google.com/view/wenbobao/dain" target="_blank">Website</a>

### Colorization & Color correction 

&nbsp;&nbsp; DeOldify: A Deep Learning based project for colorizing and restoring old images and videos

- <a href="https://github.com/jantic/DeOldify" target="_blank">Github</a>

&nbsp;&nbsp; Natron, an open-source node-based compositing software application

- <a href="https://natrongithub.github.io" target="_blank">Website</a>

&nbsp;&nbsp; Fully Automatic Video Colorization with Self-Regularization and Diversity

- <a href="https://github.com/ChenyangLEI/Fully-Automatic-Video-Colorization-with-Self-Regularization-and-Diversity" target="_blank">Github</a>

- <a href="https://www.youtube.com/watch?v=Y15uv2jnK-4>">Video</a>
 
 **Note:** This model was used only for comparison, DeOldify was primary colorization method.
 
 <p align="center"> 
     <img src="https://github.com/mburakbozbey/video-restoration/blob/master/secondaryColorizer.png" alt="img">
 </p>
 
## Procedure

 <p align="center"> 
    <img src="https://github.com/mburakbozbey/video-restoration/blob/master/diagram1.png" alt="img">
 </p>
 
Following procedure was followed in this project:

**1** - Analysis of the sample video properties for the objective and parsing it to frames

**2** - Original frames are colorized with DeOldify to improve results of the other GAN models as a preprocessing step.

**3** - <a href="https://github.com/krasserm/super-resolution/tree/previous" target="_blank">Super resolution</a> was used in local environment with Keras, 640x480 resolution was increased by factor 4 to 2560x1920.

**4** - Due to memory limitations, 2560x1920 frames were resized to 1920x1080 for video frame interpolation on <a href="https://colab.research.google.com/drive/1gzsfDV_MIdehr7Y8ZzWjTuW-mMZRP4Vy" target="_blank">Google Colab</a> that is prepared by <a href="https://github.com/styler00dollar" target="_blank">styler00dollar</a> which uses <a href="https://github.com/baowenbo/DAIN" target="_blank">Depth-Aware Video Frame Interpolation</a>. Please note that a P100 GPU in Colab is needed to allocate memory for 1080p videos.

**5** - After frame interpolation with 1920x1080 images,  resulting frames were downsized to 720x540 resolution for Super Resolution with scale 4 to achieve 4K specs(3840x2160) with horizontal padding(480x2160 + 2880x2160 + 480x2160). 

**6** - Finally, resulting frames are used to generated 4K 50fps end result, after the application of color correction & supression by using <a href="https://natrongithub.github.io" target="_blank">Natron</a>.

 <p align="center"> 
    <img src="https://github.com/mburakbozbey/video-restoration/blob/master/original.jpg" width="320" height="240" alt="img">
    <img src="https://github.com/mburakbozbey/video-restoration/blob/master/deoldify.png" width="320" height="240" alt="img">
    <img src="https://github.com/mburakbozbey/video-restoration/blob/master/corrected4K.png" width="320" height="240" alt="img">
 </p>

 
## About Original Movie

- ***Title:*** Efkarlı Sosyetede
- ***Director:*** Türker İnanoğlu
- ***Cast:*** Sadri Alışık, Filiz Akın
- ***Production Company:*** Erler Film
- ***Producer:*** Türker İnanoğlu
- ***Year:*** 1968

## Citation

**1 -** Bao, W., Lai, W.S., Ma, C., Zhang, X., Gao, Z., & Yang, M.H. (2019). Depth-Aware Video Frame Interpolation. In IEEE Conference on Computer Vision and Pattern Recognition.

**2 -** Bao, W., Lai, Zhang, X., Gao, Z., & Yang, M.H. (2018). MEMC-Net: Motion Estimation and Motion Compensation Driven Neural Network for Video Interpolation and EnhancementIEEE Transactions on Pattern Analysis and Machine Intelligence.

**3 -** Lei, C., & Chen, Q. (2019). Fully Automatic Video Colorization With Self-Regularization and Diversity. In The IEEE Conference on Computer Vision and Pattern Recognition (CVPR).

## Disclaimer (EN/TR)

- This repository is prepared for the review of recent the state-of-art methods that are available for video restoration on Github with nonprofit educational purposes only. The sample video was used to reproduce the whole pipeline while respecting the copyright holders in terms of fair use.   

- Yapılan çalışma Github üzerinde yalnızca kar amacı gütmeyen eğitim amaçları göz edilerek video restorasyonu için mevcut olan en son teknolojik yöntemlerin gözden geçirilmesi için hazırlanmıştır. Kullanılan eser, adil kullanım kapsamında telif hakkı sahiplerine saygı gösterilerek işlenmiştir.
