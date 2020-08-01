# MNIST-CNN-PYNQ
2020 New Engineering Alliance-Xilinx summer school project.<br>
Handwritten numbers recognition based on PYNQ-Z2 is realized.<br>
References for this project [Github](https://github.com/fpgasystems/spooNN)

# what is MNIST
MNIST data set is classic in the machine learning field. It is composed of 60000 training samples and 10000 test samples. Each sample is a 28 * 28 pixel gray handwritten number image.<br> 

# Step
## 1 Training CNN
In tensorflow framework, we trained a traditional CNN model(4 convolution-layer, 2 pooling-layer and 2 full connection-layer) with MNIST data set. Finaly, the handweitten numbers recognition accuracy is 99%. We transform the super parameters and weight parameters of themodel into .h files.

## 2 HLS and Overlay
Generating IP based on C + + in VIVADO HLS, building Block Desgin in VIVADO and then generating bitstream and .tcl file.

## 3 PYNQ-Z2
Based on Python productivity for Zynq open-source frame, we verified this project on PYNQ-Z2, the accuracy is 97.82% about 5000 handwritten number image.
