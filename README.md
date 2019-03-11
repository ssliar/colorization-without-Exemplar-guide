# Colorization-without-Exemplar-guide
   轻量的图像自动上色模型，支持实时的视频上色.

Environments:
---- 
- pytorch 0.4.1
- python 3.6
- ubuntu 16.04

Keys:
---
- 类似[bicyclegan](https://arxiv.org/abs/1711.11586),定义一个轻量级的生成器G,跟一个判别器D,以及一个VAE编码器。
- 将RGB图像转化为YCbCr格式，Y通道作为输入，CbCr通道作为输出
- 添加额外的Perceptual Loss

Test On Image:
----
```
    python testImage.py --input input_image
```


Test On Picture:
----
```
    python testVideo.py --input video_input
```

Results:
----
![]
