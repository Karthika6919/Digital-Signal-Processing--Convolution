# Digital-Signal-Processing--Convolution
## Aim:
                  To perform linear convolution using MAT LAB.
## Software Required:
MAT LAB R2012
## Algorithm:
Step 1: Open mat lab. Write the program.

Step 2: Read the first input sequence.

Step 3: Read the second impulse sequence.

Step 4: Plot the input sequences with x-label and y-label with suitable title. 

Step 5: Perform convolution for both the sequences using conv2() function.
  
Step 6: Plot the sequence with x-label and y-label with suitable title

Step 7: Terminate the program.

## PROGRAM: 
```
clc;%clear screen
clear all;% clear screen
close all;%close all figure windows
a= input('enter the starting x(n)');
x=input('enter the x(n) sequence');
n=a:1:length(x)+a-1;
figure(1);
stem(n,x);
xlabel('time');
ylabel('amplitude');
title('input sequence');

b=input('enter the starting h(n)');
y=input('enter the h(n) sequence');
m=b:1:length(y)+b-1;
figure(2);
stem(m,y);
xlabel('time');
ylabel('amplitude');
title('impluse response')

z=conv2(x,y);
n1=a+b:1:length(z)+a+b-1;
figure(3);
stem(n1,z);
xlabel('time');
ylabel('amplitude')
title('linear convolution');
```
## OUTPUT:
<img width="1818" height="914" alt="Screenshot 2026-02-09 224740" src="https://github.com/user-attachments/assets/2823b41d-f84b-403e-a4b1-95e96738299b" />
<img width="1777" height="900" alt="Screenshot 2026-02-09 224801" src="https://github.com/user-attachments/assets/ed8578a4-6d50-407e-9f76-bc51370d5dcb" />
<img width="1854" height="904" alt="Screenshot 2026-02-09 224824" src="https://github.com/user-attachments/assets/ab91e184-616b-433a-8384-79214422c1fd" />


## RESULT:
![WhatsApp Image 2026-04-03 at 11 54 59 AM](https://github.com/user-attachments/assets/4fb6d533-65f4-44b7-bf54-5e81f1d5b5b6)

