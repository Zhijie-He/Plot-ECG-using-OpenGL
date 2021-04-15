# Plot-ECG-using-OpenGL
1.get the dataset from biosppy 

2.plot the real-time ECG images using OpenGL

References:

https://github.com/PIA-Group/BioSPPy

https://biosppy.readthedocs.io/en/stable/

https://en.wikipedia.org/wiki/Electrocardiography#Electrocardiogram_grid

![image](https://user-images.githubusercontent.com/80511292/114937665-5cfa4a80-9e3e-11eb-9b77-a89118a22245.png)

The upper line is one second of ECG signal

Below line is all the signal 





## Project Requirements:
Plot this electrocardio graphic (ECG) signal in a graphic with the following specifications:

1.The window should correspond to 1 second of signal and it should simulate an online acquisition, with new samples beingdrawn on the right. You should keep a vector with only the visible part of the signal.

2.To simulate a continuous acquisition, once you have drawn all the samples you restart on the beginning of the signal (you will need to create a circular buffer).

3.The framebuffer refreshing rate should be the same as the one used for refreshing the screen of your computer. This will allow you to know how you should shift your circular buffer for each draw.

4.Draw the signal in standard ECG grid, specifications are given in https://en.wikipedia.org/wiki/Electrocardiography#Electrocardiogram_grid and the lines should be drawn in light pink color. The amplitudes should range from −0.5 mV to 5 mV. The ECG signal is the direct output of an analog to digital converter, its amplitude is quantized in integer values from 0 to 4095. You can consider that the quantizer is uniform (constant steps) with 0 mV corresponding to the value 2047 and each integer value step corresponding to a change of 0.01 mV.

