# FM-using-Python

Aim


To implement and analyze frequency modulation (FM) using Python's NumPy and Matplotlib libraries. 

Apparatus Required

1.	Software: Python with NumPy and Matplotlib libraries
2.	Hardware: Personal Computer
  
Theory

Frequency Modulation (FM) is a method of transmitting information over a carrier wave by varying its frequency in accordance with the amplitude of the input signal (message signal). The frequency of the carrier wave is varied according to the instantaneous amplitude of the message signal. The general form of an FM signal is:



Algorithm


1.	Initialize Parameters: Set the values for carrier frequency, message frequency, sampling frequency, and frequency deviation.
2.	Generate Time Axis: Create a time vector for the signal duration.
3.	Generate Message Signal: Define the message signal as a cosine wave.
4.	Compute the Integral of the Message Signal: Calculate the integral of the message signal over time.
5.	Generate FM Signal: Apply the FM modulation formula to obtain the modulated signal.
6.	Plot the Signals: Use Matplotlib to plot the message signal, carrier signal, and modulated signal.

Program
```
Am = 5.2;
fm = 417;
Ac = 10.4;
fc = 4170;
fs = 41700;
t = 0:1/fs:3/fm;
m = Am * cos(2 * %pi * fm * t);
subplot(3,1,1);
plot(t, m);
c = Ac * cos(2 * %pi * fc * t);
subplot(3,1,2);
plot(t, c);
kf = 5.1; 
efm = Ac * cos(2 * %pi * fc * t + kf * sin(2 * %pi * fm * t));
subplot(3,1,3);
plot(t, efm);
```

Output Waveform
![WhatsApp Image 2025-11-24 at 23 04 49_bbd37d2b](https://github.com/user-attachments/assets/6b9e6e8a-264e-4d4f-8b2c-b50a377030bb)


Tabular Column
![WhatsApp Image 2025-12-05 at 12 14 01_4db949dd](https://github.com/user-attachments/assets/e25e7395-a8e3-430d-a114-6970dae9558c)



Calculation

![WhatsApp Image 2025-12-05 at 12 14 03_36d5771d](https://github.com/user-attachments/assets/b1bd2894-0694-4290-b37b-14ce6e3ea639)



Result
The message signal, carrier signal, and frequency modulated (FM) signal will be displayed in separate plots. The modulated signal will show frequency variations corresponding to the amplitude of the message signal.



The message signal, carrier signal, and frequency modulated (FM) signal will be displayed in separate plots. The modulated signal will show frequency variations corresponding to the amplitude of the message signal.
