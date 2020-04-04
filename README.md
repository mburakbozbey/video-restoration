# Video Restoration with Pretrained DL Models

An end-to-end video restoration process with the-state-of-art deep neural network models was tested on <a href="https://www.youtube.com/watch?v=5yeNO-l7OLc">sample video</a>

### Resources

- Google Colab
- Anaconda
- Local:

**OS**: Windows 10 Home 64-bit

**GPU**: GeForce GTX 1060 Max-Q 

**CPU**: Intel i7-7700HQ

**RAM**: 16GB


## Sample Video Properties

- ***Length*** : 00:00:49
- ***Width*** : 640
- ***Height*** : 480
- ***Frame per second***: 25
- ***Number of frames***: 2726
- ***Format*** : .mp4

## Diagram

 <p align="center"> 
    <img src="https://github.com/mburakbozbey/video-restoration/blob/master/diagram.png" alt="img">
 </p>
 
## Methods
### Super Resolution:

- EDSR, WDSR and SRGAN for single image super-resolution that requires the Keras Tensorflow backend.
Github: https://github.com/krasserm/super-resolution/tree/previous

### Video frame interpolation

- Depth-Aware Video Frame Interpolation (CVPR 2019): <a href="https://github.com/baowenbo/DAIN" target="_blank">Github</a>, <a href="https://sites.google.com/view/wenbobao/dain" target="_blank">Website</a>

### Colorization

- DeOldify: A Deep Learning based project for colorizing and restoring old images (and video!)

<a href="https://github.com/jantic/DeOldify" target="_blank">Github</a>

- Fully Automatic Video Colorization with Self-Regularization and Diversity

<a href="https://github.com/ChenyangLEI/Fully-Automatic-Video-Colorization-with-Self-Regularization-and-Diversity" target="_blank">Github</a>
<a href="https://www.youtube.com/watch?v=Y15uv2jnK-4>">Video</a>
 
 ***Note:*** This model was used only for comparison, DeOldify was primary colorization method.
 
- Color correction: Natron, an open-source node-based compositing software application
<a href="https://natrongithub.github.io" target="_blank">Website</a>

## Results

- <a href="https://www.youtube.com/watch?v=5yeNO-l7OLc">Original Video</a>
- Final Postprocessing (4K + 50FPS) ( will be added soon)
- Other Color Videos ( will be added soon)

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

- Yapılan çalışma Github üzerinde yalnızca kar amacı gütmeyen eğitim amaçları göz edilerek video restorasyonu için mevcut olan en son teknolojik yöntemlerin gözden geçirilmesi için hazırlanmıştır. Kullanılan eser, adil kullanım kapsamında telif hakkı sahiplerine saygı gösterilerek kullanılmıştır.
