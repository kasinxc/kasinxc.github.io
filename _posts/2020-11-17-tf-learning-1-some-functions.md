---
layout: default
title: TF Functions in Development
icategories: ML
tags: [Newbie, tensorflow]
---
# TF Functions in Developement

### Tensorflow functions

#### tf.divide

```python
tf.divide(x, y, name=None)
```python

element-wise x divided by y.

[tf.divide](https://docs.w3cub.com/tensorflow~python/tf/divide/) 

#### tf.reduce_sum

```python
tf.reduce_sum(
    input_tensor,
    axis=None,
    keepdims=None,
    name=None,
    reduction_indices=None,
    keep_dims=None
)
```

Computes the sum of elements across dimensions of a tensor.

##### Example:

```python
x = tf.constant([[1, 1, 1], [1, 1, 1]])
tf.reduce_sum(x)  # 6
tf.reduce_sum(x, 0)  # [2, 2, 2]
tf.reduce_sum(x, 1)  # [3, 3]
tf.reduce_sum(x, 1, keepdims=True)  # [[3], [3]]
tf.reduce_sum(x, [0, 1])  # 6
```

[tf.reduce_sum](https://docs.w3cub.com/tensorflow~python/tf/reduce_sum/)

### Keras functions


### JAX functions

#### 什么是JAX?

袁进辉：“tensorflow 主打lazy，偏functional的思想，但实现的臃肿面目可憎；pytorch主打eager，偏imperative编程，但内核简单，可视作支持gpu的numpy加上autograd。JAX则像是这两个框架的混合体，取了tensorflow的functional和pytorch的精简，支持GPU的numpy，具有autograd功能，追求函数式编程的思想，强调无状态，immutable，加上JIT修饰符之后就是lazy，可以使用xla对计算流程进行静态分析和优化，不带JIT也可以像pytorch那种命令式编程和eager执行。”

蔡善清：“简单的说 就是GPU加速，支持自动微分(autodiff)的numpy”： numpy不支持GPU或其他硬件加速器，也没有对back probagation的支持，但是底层且灵活。”







$IDF = log(\frac{语料库的文档总数}{包含词条w的文档数+1})$















## Reference

[【知乎】如何评价谷歌开源的Tensorflow简化库JAX](https://www.zhihu.com/question/306496943)


----
<a href="{{ site.baseurl }}/index.html">Home</a>
