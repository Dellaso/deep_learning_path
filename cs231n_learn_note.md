
## cs231n hard point learn note
>这里用来记录我在学习cs231n过程中的困惑点和难点笔记，而非大纲要点的笔记。视频教程中有些知识点并没有详细阐述，需要我自己查资料消化。
>
>笔记中的粗体是我还依然困惑的，后续会抽时间解惑。若有网友能解惑，欢迎Pull requests

### 一、简介
### 二、图像分类
1. [KNN的原理是什么？A君解释](https://blog.csdn.net/jack339083590/article/details/79209165)

    etc. [B君解释](https://www.cnblogs.com/jtianwen2014/p/4249003.html)、[C君解释](https://cuijiahua.com/blog/2017/11/ml_1_knn.html)

2. KNN代码看不懂。

  train:存储每个已知图及其标签。O(1)

  predict:要预测的图和每个已知的图对比一遍，差距最小的即属于同一类标签。O(n)

3. KNN区域决策图看不懂。

  解：每个点是已知物体的分类，背景色块是决策区域。根据已知点预测其它区域的类别。
（[vision demo](http://vision.stanford.edu/teaching/cs231n-demos/knn/) **这个demo怎么做？**）

4. **Distance Metic: Mahatto-distance vs Euclidean-distance 的区别?**

  （即：距离差的绝对值的和 vs 距离差的平方和的平方根）
  
5. curse of dimensionality 不理解

   解：决策区域是根据已知的训练点来划分的。所以理论上，训练点越多，决策区域的划分越精确。可是随着维度的增加，想要获得同样精确度的训练点数量会指数级增长，
   运算量就会爆炸，所以不好。这里的维度是指决策指标，大于3的情况也很多。

