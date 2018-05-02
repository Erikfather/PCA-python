# 基于python的PCA人脸识别算法
## 结果如下：

### 具体代码见：Face_Rec.py
   当每个人只选择一张图片进行训练时，训练集只有40张，所以这种情况下最多只能降到40维（即主成分为40），故为不失一般性，我只比较了降到10、20、30、40维情况下，每个人选择1-9张图片进行训练的识别准确率，结果如下：
![image](https://github.com/Erikfather/PCA-python/blob/master/results/result.png)
#### 下面的图像更直观的表现出各维度下，选择不同照片张数的识别准确率。
![image](https://github.com/Erikfather/PCA-python/blob/master/results/Figure_10维.png)
![image](https://github.com/Erikfather/PCA-python/blob/master/results/Figure_20维.png)
![image](https://github.com/Erikfather/PCA-python/blob/master/results/Figure_30维.png)
![image](https://github.com/Erikfather/PCA-python/blob/master/results/Figure_40维.png)
![image](https://github.com/Erikfather/PCA-python/blob/master/results/Figure_%E6%AF%94%E8%BE%83.png)




### 通过上面的图像我们可以看出：
   （1）在降到相同维度下（即相同主成分大小下），每个人选择的照片张数越多，即训练集越多，准确率越高。在每个人选择照片张数大于等于5时，即训练集达到整个样本数据集的一半时，准确率达到90%以上；<br>
   （2）在每个人选择照片张数相同情况下，即训练数据集大小相同情况下，降到的维数越高，即主成分越多，准确率越高；<br>
   （3）总体上来说，识别准确率整体上呈现上升趋势。随着训练数据集规模的增大而升高，同时也随着主成分大小的增大而增大。<br>
