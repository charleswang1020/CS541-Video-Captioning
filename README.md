# CS541-2019S-Video Captioning
WPI CS 541 Deep Learning Project 

## Description
Captioning videos is to make video collection more accessible to human users and for making video content more accessible to the visually impaired. This task is to do the visual encoding into language. It focus on the task of expressing the visual content of the videos in the English language. One of the more common frameworks for attempting this task is an encoder-decoder framework. This framework is used to implement and train from scratch a video captioning RNN (GAN) to investigate a current state of the art technique. To improve the performance of the technique we experiment with augmenting this approach with some of the newest pre-trained CNN models for our initial image feature extraction and use modern regularization methods. To demonstrate the effectiveness of our approach we test our method on the MSR-VTT dataset.

## Prerequisite
OpenCV (Python)
* pip install python-opencv

## Method
We propose a CNN-RNN based approach using the encoder-decoder framework. This category of approaches leverage advanced pretrained CNNs to efficiently and accurately preprocess the image component of the video data and trains an RNN to collect data from multiple frames and then generate the sentences. We augment this approach with some of the newest pretrained CNN models for our initial image feature extraction.<br>
CNN-RNN framework whose the first high-level features are extracted from a CNN trained on the image classification task, and then a recurrent model learns to predict subsequent words of a caption conditioned on image features and previously predicted words.<br>

![](/images/Network_diagram.JPG)

## Data Source
Compiled from [1], [2], and dataset search

|    Dataset  | Domain | Classes| Videos | Clips | Sentence|  Words  |  Vocab | Len(hrs) |
|:-----------:|:------:|:------:|:------:|:-----:|:-------:|:-------:|:------:|:--------:|
|     MSCD    |  Open  |   218  |  1,970 | 1,970 |  70,028 | 607,339 | 13,010 |     5    |
|    MSR-VTT  |  Open  |   20   |  7,180 | 10,000| 200,000 |1,856,523| 29,316 |     5    |

## Video Demo
![](/images/Screenshot_Demo.JPG)

## Presentation Slides

## References
[1] Aafaq,  Nayyer,  Gilani,  Syed  Zulqarnain,  Liu,  Wei,  and Mian,  Ajmal. Video description:   a survey of methods, datasets and evaluation metrics. arXiv preprint arXiv:1806.00186, 2018.

[2] Gella, Spandana, Lewis, Mike, and Rohrbach, Marcus.  A dataset for telling the stories of social media  videos. In Proceedings of the 2018 Conference on Empirical Methods in Natural Language Processing, pp. 968–974, 2018

[3] Lavie, Alon and Agarwal, Abhaya.  Meteor: An automatic metric for mt evaluation with high levels of correlation with human judgments.   In Proceedings of the Second Workshop on Statistical Machine Translation,  StatMT’07, pp. 228–231, 2007.

[4] Vedantam, Ramakrishna, Lawrence Zitnick, C., and Parikh, Devi.  Cider: Consensus-based image description evaluation.  In The IEEE Conference on Computer Vision and Pattern Recognition (CVPR), June 2015.

[5] Venugopalan,  Subhashini,  Rohrbach,  Marcus,  Donahue, Jeffrey, Mooney, Raymond, Darrell, Trevor, and Saenko, Kate. Sequence to sequence - video to text. In The IEEE International Conference on Computer Vision (ICCV), December 2015.

[6] Xu,  Jun,  Mei,  Tao,  Yao,  Ting,  and  Rui,  Yong.   Msr-vtt: A large video description dataset for bridging video and language.  In The IEEE Conference on Computer Vision and Pattern Recognition (CVPR), June 2016
