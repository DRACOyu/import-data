import-data
====

three ways to import data

# 1,Preloaded data: 预加载数据
 <br>
'''
    import tensorflow as tf  
    # 设计Graph  
    x1 = tf.constant([2, 3, 4])  
    x2 = tf.constant([4, 0, 1])  
    y = tf.add(x1, x2)  
    # 打开一个session --> 计算y  
    with tf.Session() as sess:  
        print sess.run(y)  
'''
# 2,

# 3,

