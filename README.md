# Music_Classification

目标: 英特尔杯人工智能项目比赛。

**项目说明:**  
    
![](https://img.shields.io/badge/language-python-green.svg)
![](https://img.shields.io/badge/package-numpy-redgreen.svg)
![](https://img.shields.io/badge/package-librosa-redgreen.svg)
![](https://img.shields.io/badge/package-sklearn-redgreen.svg)  
    
**比赛网址:**  
https://cpipc.chinadegrees.cn/cw/hp/2c9088a5696cbf370169a3f8101510bd

**技术实现**
所需环境如下：
1. 基于python语言开展项目。
2. librosa库包进行音频解析。
3. csv库包进行数据的临时存取。
4. numpy库包进行数据的计算。
5. pandas库包进行csv数据的读写操作。
6. os库包进行系统文件的增删。
7. keras库包进行深度学习网络的搭建。

我们使用python语言进行项目的编程，在PyCharm软件上集合所需库包搭建项目。将主要技术实现步骤概括如下：  
1、训练数据, 我们将使用著名的GITZAN数据集进行案例研究，该数据集曾用于G.Tzanetakis和P.Cook在IEEE Transactions on Audio and Speech Processing 2002 中的“ 音频信号的音乐类型分类”。数据集由每30秒长的1000个音轨组成，它包含10种类型：蓝调、古典、乡村、迪斯科、嘻哈、爵士、雷鬼、摇滚、金属和流行音乐，每种类型包含100个声音片段。  
2、将音频片段进行解析，分解成26个变量，归一化后存储在本地的csv文件中，以供后续深度学习网络训练使用。  
3、数据预处理，去除不需要的字段，将数据缺失的字段进行补齐，将类别名转换为相应的标签等操作。  
4、模型搭建, 我们采用256/128/32/10四层全连接神经网络, 最终通过softmax函数输出识别的音乐分类在各个流派的概率，并输出概率最大的音乐流派。  
5、存储训练好的权重文件于本地，用于后期进行实时音频检测使用。  
6、使用深度学习网络读取权重文件，并开启耳麦进行环境声音采集，实时进行音频的计算，直至分类形成，并输出。  

 ![image](https://github.com/763678968/Music_Classification/blob/master/1f4a1e7f3bb708d7ef63de44b358920.png)
    
**结语:**
    
    Fighting！！！
