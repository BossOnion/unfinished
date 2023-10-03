# unfinished！！！未完成！！！
# pynq_cnn_accelerator
【mdoel_training_CPU】使用CPU搭建、训练、转换、量化LeNet-5模型  
——模型结构： 
————INPUT(28x28x1)  
————CONV1（28x28x8，3x3，ReLU，Padding）  
————POOL1（14x14x8，2x2,MaxPooling）  
————CONV2（14x14x6，3x3，ReLU，Padding）  
————POOL2（7x7x16，2x2,MaxPooling）  
————FC1（7x7x16,120,ReLU）  
————FC2（120,10,Softmax）  
——h5格式模型准确率：训练集99.31%，测试集98.88%，大小1252KB  
——tflite格式模型准确率：测试集98.54%，大小407KB  
——量化后tflite格式模型准确率：测试集98.68，大小106KB，whght-int8，bias-float32  
【model_training_GPU】  
——模型结构：同CPU training  
——h5格式模型准确率：训练集99.26%，测试集99.06%，大小1249KB  
——tflite格式模型准确率：测试集98.98%，大小406KB  
——量化后tflite格式模型准确率：测试集98.99，大小105KB，whght-int8，bias-float32  
