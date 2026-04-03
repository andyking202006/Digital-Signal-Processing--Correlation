# Digital-Signal-Processing--Correlation
## AIM:
To generate discrete auto correlation and cross correlation of signals using MATLAB.
## APPARATUS REQUIRED:
MATLAB R2012.
## ALGORITHM:
Step 1: Open matlab. Write the program.

Step 2: Read the input sequence 1 and input sequence 2 sequence.

Step 3: Perform auto correlation and cross correlation for both the sequences. 

Step 4: Plot the output sequence with x-label and y-label with suitable title.

Step 5: Terminate the program.


## PROGRAM: 
clc;
clear all;
close all;

% INPUT SIGNAL-1
a = input('enter the starting x(n)');
x = input('Enter the x(n) sequence');
n = a : 1 : length(x) + a - 1;
figure(1)
stem(n,x)
xlabel('Time')
ylabel('Amplitude')
title('Input Signal-1')

% INPUT SIGNAL-2
b = input('enter the starting y(n)');
y = input('Enter the y(n) sequence');
m = input('enter the ending y(n)');
n1 = b : 1 : length(y) + b - 1;
figure(2)
stem(n1,y)
xlabel('Time')
ylabel('Amplitude')
title('Input signal-2')

% DISCRETE AUTO CORRELATED SIGNAL
Out1 = xcorr(x,x);
n2 = a - m : 1 : length(Out1) + a - m - 1;
figure(3)
stem(n2,Out1)
xlabel('Time')
ylabel('Amplitude')
title('Discrete auto correlated waveform')

% DISCRETE CROSS CORRELATED SIGNAL
Out2 = xcorr(x,y);
n3 = a - m : 1 : length(Out2) + a - m - 1;
figure(4)
stem(n3,Out2)
xlabel('Time')
ylabel('Amplitude')
title('Discrete cross correlated waveform')

## OUTPUT:
![WhatsApp Image 2026-02-22 at 12 23 35](https://github.com/user-attachments/assets/0f779162-aa6a-490d-9f2d-c43a7478aa3e)
![WhatsApp Image 2026-02-22 at 12 23 3](https://github.com/user-attachments/assets/6e3eeaac-1118-4524-b7d2-22e90ad15aa4)
![WhatsApp Image 2026-02-22 at 12 23](https://github.com/user-attachments/assets/69fe7191-a81c-4eae-8344-7cb11c8f3b69)
![WhatsApp Image 2026-02-22 at ](https://github.com/user-attachments/assets/b79b7ded-5082-4796-acc6-6a29b5cfce00)

## RESULT:
![WhatsApp Image 2026-04-03 at 12 24 14](https://github.com/user-attachments/assets/c8e3da7c-26b3-4afa-82a7-327dc3ccaee2)



