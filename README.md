# TensorFow install for RTX3090

## 1. Download and install VSCODE 

https://code.visualstudio.com/

## 2. Install CUDA and Cudnn

- OS : Windows10

- VGA : RTX 3090

- VGA Driver : 456.81

- Cuda 설치 :   (cuda 11.1 업데이트된 최신버전)

- Cudnn 설치 : cudnn-11.1-windows-x64-v8.0.4.30(cudnn)

- Anaconda 설치

- 가상환경 생성 : conda create -n TF_test_RTX3090 python=3.8 -> conda activate TF_test_RTX3090

- tensorflow-gpu 설치 : pip install tf-nightly-gpu==2.5.0.dev20210107 

- Numpy 설치 : conda install numpy (pip로 설치시 에러발생된적 있음)

- Keras 설치 : pip install keras (nightly 버전으로 keras 별도설치)

- pytorch 설치 할 경우 : conda install pytorch torchvision torchaudio cudatoolkit=11.1 -c pytorch


## 5. Simple test code
```
import tensorflow as tf

hello = tf.constant('Hello, TensorFlow!')
print(hello.numpy())
#'Hello, TensorFlow!'

a = tf.constant(10)
b = tf.constant(32)
print((a + b).numpy())
```

```
import tensorflow as tf  
import numpy as np  
from tensorflow import keras  
model = tf.keras.Sequential([keras.layers.Dense(units=1, input_shape=[1])])
```

