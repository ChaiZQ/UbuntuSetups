aemc2@aemc2:~$ export PATH=/usr/local/cuda-8.0/bin${PATH:+:${PATH}}
aemc2@aemc2:~$ export LD_LIBRARY_PATH=/usr/local/cuda-8.0/lib64${LD_LIBRARY_PATH:+:${LD_LIBRARY_PATH}}


aemc2@aemc2:~$ cd /usr/local/cuda-8.0/samples/1_Utilities/deviceQuery
aemc2@aemc2:~$ sudo make
aemc2@aemc2:~$ ./deviceQuery 
### Result = PASS

aemc2@aemc2:~$ nvidia-smi
+-----------------------------------------------------------------------------+
| NVIDIA-SMI 384.130                Driver Version: 384.130                   |
|-------------------------------+----------------------+----------------------+
| GPU  Name        Persistence-M| Bus-Id        Disp.A | Volatile Uncorr. ECC |
| Fan  Temp  Perf  Pwr:Usage/Cap|         Memory-Usage | GPU-Util  Compute M. |
|===============================+======================+======================|
|   0  GeForce GTX 108...  Off  | 00000000:01:00.0  On |                  N/A |
|  0%   39C    P8    17W / 275W |    423MiB / 11169MiB |      0%      Default |
+-------------------------------+----------------------+----------------------+
                                                                               
+-----------------------------------------------------------------------------+
| Processes:                                                       GPU Memory |
|  GPU       PID   Type   Process name                             Usage      |
|=============================================================================|
|    0      1088      G   /usr/lib/xorg/Xorg                           283MiB |
|    0      1890      G   compiz                                       137MiB |
+-----------------------------------------------------------------------------+


aemc2@aemc2:~$ tar xvzf cudnn-8.0-linux-x64-v5.1.tgz
aemc2@aemc2:~$ cd cuda
aemc2@aemc2:~$ sudo cp include/* /usr/local/cuda-8.0/include/
aemc2@aemc2:~$ sudo cp lib64/* /usr/local/cuda-8.0/lib64/

aemc2@aemc2:~$ nvcc --version
nvcc: NVIDIA (R) Cuda compiler driver
Copyright (c) 2005-2016 NVIDIA Corporation
Built on Tue_Jan_10_13:22:03_CST_2017
Cuda compilation tools, release 8.0, V8.0.61
