# TensorFow install for GTX3090

## 1. Download and install VSCODE 

https://code.visualstudio.com/

## 2. Install CUDA and Cudnn

OS : Windows10

VGA : RTX 3090

VGA Driver : 456.43

Cuda 설치 :   (cuda 11.0 업데이트된 최신버전)

Cudnn 설치 : cudnn-11.0-windows-x64-v8.0.3.33(cudnn)

Anaconda 설치

가상환경 생성 : conda create -n env_name python=3.8 -> conda activate env_name

tensorflow-gpu 설치 : pip install tf-nightly-gpu==2.5.0.dev20201102

conda install pytorch torchvision torchaudio cudatoolkit=11.0 -c pytorch



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

## References
- https://koos808.tistory.com/41
