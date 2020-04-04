# Video Restoration with Pretrained DL Models

An end-to-end video restoration process with the-state-of-art deep neural network models was tested on <a href="https://www.youtube.com/watch?v=5yeNO-l7OLc">sample video</a>

## Results

- <a href="https://www.youtube.com/watch?v=UtgXiHRS_nc">Original vs Final</a>
- <a href="https://www.youtube.com/watch?v=qqaCTEEdVYA">Final Postprocessing (4K + 50FPS) </a>
- <a href="https://www.youtube.com/watch?v=qjg2-W09Yp0">Fully Automatic Video Colorization with Self-Regularization and Diversity</a>

### Resources

- Google Colab
- Anaconda
- Local

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

## Diagram

 <p align="center"> 
    <img src="https://github.com/mburakbozbey/video-restoration/blob/master/diagram1.png" alt="img">
 </p>
 
## Methods
For reproduction of the results, following procedure was used:
1 - Analyzing sample video properties and parsing to frames
2 - Super resolution repository was used in local environment with Keras
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

 <p align="center"> 
    <img src="https://github.com/mburakbozbey/video-restoration/blob/master/original.jpg" width="320" height="240" alt="img">
    <img src="https://github.com/mburakbozbey/video-restoration/blob/master/deoldify.png" width="320" height="240" alt="img">
    <img src="https://github.com/mburakbozbey/video-restoration/blob/master/corrected4K.png" width="320" height="240" alt="img">
 </p>

&nbsp;&nbsp; Fully Automatic Video Colorization with Self-Regularization and Diversity

- <a href="https://github.com/ChenyangLEI/Fully-Automatic-Video-Colorization-with-Self-Regularization-and-Diversity" target="_blank">Github</a>

- <a href="https://www.youtube.com/watch?v=Y15uv2jnK-4>">Video</a>


    <img src="https://github.com/mburakbozbey/video-restoration/blob/master/secondaryColorizer.png" alt="img">

 
 ***Note:*** This model was used only for comparison, DeOldify was primary colorization method.
 
### About Original Movie

- ***Title:*** Efkarlı Sosyetede
- ***Director:*** Türker İnanoğlu
- ***Cast:*** Sadri Alışık, Filiz Akın
- ***Production Company:*** Erler Film
- ***Producer:*** Türker İnanoğlu
- ***Year:*** 1968

## References

Bao, W., Lai, W.S., Ma, C., Zhang, X., Gao, Z., & Yang, M.H. (2019). Depth-Aware Video Frame Interpolation. In IEEE Conference on Computer Vision and Pattern Recognition.

Bao, W., Lai, Zhang, X., Gao, Z., & Yang, M.H. (2018). MEMC-Net: Motion Estimation and Motion Compensation Driven Neural Network for Video Interpolation and EnhancementIEEE Transactions on Pattern Analysis and Machine Intelligence.

Lei, C., & Chen, Q. (2019). Fully Automatic Video Colorization With Self-Regularization and Diversity. In The IEEE Conference on Computer Vision and Pattern Recognition (CVPR).

## Disclaimer (EN/TR)

- This repository is prepared for the review of recent the state-of-art methods that are available for video restoration on Github with nonprofit educational purposes only. The sample video was used to reproduce the whole pipeline while respecting the copyright holders in terms of fair use.   

- Yapılan çalışma Github üzerinde yalnızca kar amacı gütmeyen eğitim amaçları göz edilerek video restorasyonu için mevcut olan en son teknolojik yöntemlerin gözden geçirilmesi için hazırlanmıştır. Kullanılan eser, adil kullanım kapsamında telif hakkı sahiplerine saygı gösterilerek işlenmiştir.
