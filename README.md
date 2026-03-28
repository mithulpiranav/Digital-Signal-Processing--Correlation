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

<img width="1600" height="1322" alt="image" src="https://github.com/user-attachments/assets/0df1cf44-a36e-469c-8a0e-dc7e08e38c45" />

<img width="1600" height="1485" alt="image" src="https://github.com/user-attachments/assets/d8d9cdd0-70d5-4c32-a1e3-982c9fc07231" />

<img width="1600" height="1376" alt="image" src="https://github.com/user-attachments/assets/b42e8867-9835-47ce-9578-82a1bb296f1f" />

<img width="1600" height="1382" alt="image" src="https://github.com/user-attachments/assets/ef379d7b-5532-478a-aa0d-296c469f71a3" />


## RESULT:

![Img](https://github.com/user-attachments/assets/63b8fff2-b077-46bc-b159-6bb707bd0b4f)


