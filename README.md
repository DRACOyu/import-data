import-data
====

three ways to import data

# 1,Preloaded data: 预加载数据
 
```python
    import tensorflow as tf  
    # 设计Graph  
```
# 2,cifar10为例，读取bin二进制文件
首先直接读取路径下的文件，采用tf.FixedLengthRecordReader读取固定长度（标签+图片）的字节数信息，<br>
reader.read读取读取队列中的数据，<br>
tf.decode_raw将字符串转化为张量,再使用tf.slice分割字符，转化类型等等 <br>
最后使用tf.train.batch生成batch输出，最后可能加一个one-hot向量转化

# 3,Reading from file: 从文件中直接读取

