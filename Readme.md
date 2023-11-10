| **Index** |                                                                                                                                                                                      |              |             |
| :-------: | :----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | :----------- | :---------- |
| **S.No.** | **Name of the Experiments**                                                                                                                                                          | **Page No.** | **Remarks** |
|   **1**   | **Matlab code for Generation of unit impulse signal with delay and advance**                                                                                                         |              |             |
|   **2**   | **Matlab code for Generation of unit step signal with delay and advance**                                                                                                            |              |             |
|   **3**   | **Matlab code for Generation of unit ramp signal with delay and advance**                                                                                                            |              |             |
|   **4**   | **y=sin(t)**                                                                                                                                                                         |              |             |
|   **5**   | <p>**y=4\*sin(t)^2** </p><p></p><p>**-2\*pi<t<2\*pi**</p>                                                                                                                            |              |             |
|   **6**   | <p>**y=4\*sin(ωt)+cos(ωt)**</p><p></p><p>**-2\*pi<t<2\*pi**</p>                                                                                                                      |              |             |
|   **7**   | **y=cos(t)**                                                                                                                                                                         |              |             |
|   **8**   | <p>**y=t==0**</p><p></p><p>**-2\*pi<t<2\*pi**</p>                                                                                                                                    |              |             |
|   **9**   | <p>**y=4\*cos(t)^2**</p><p></p><p>**-2\*pi<t<2\*pi**</p>                                                                                                                             |              |             |
|  **10**   | <p>**Step =t>=0**</p><p></p><p>**t=-1:0.109:1**</p>                                                                                                                                  |              |             |
|  **11**   | <p>**y=t\*ramp**</p><p></p><p>**ramp=t>=0**</p><p></p><p>**t=-1:0.1:1**</p>                                                                                                          |              |             |
|  **12**   | **When x(n)={1 ; n >= 0 , 0 ; n <0**                                                                                                                                                 |              |             |
|  **13**   | **x(n-2)={1 ; n>=0 , 0 ; n<0**                                                                                                                                                       |              |             |
|  **14**   | **x(n+2)={1 ; n>=0 , 0 ; n<0**                                                                                                                                                       |              |             |
|  **15**   | **x(n)={n ; n>0 , 0 ; n=<0**                                                                                                                                                         |              |             |
|  **16**   | **x(n-2)={n ; n>0 , 0 ; n=<0**                                                                                                                                                       |              |             |
|  **17**   | **x(n+2)={n ; n>0 , 0 ; n=<0**                                                                                                                                                       |              |             |
|  **18**   | **x(n)={1 ; n=0 , 0 ; otherwise**                                                                                                                                                    |              |             |
|  **19**   | **x(n-5)={1 ; n=0 , 0 ; otherwise**                                                                                                                                                  |              |             |
|  **20**   | **x(n+5)={1 ; n=0 , 0 ; otherwise**                                                                                                                                                  |              |             |
|  **21**   | **x(n+8)={1 ; n=0 , 0 ; otherwise**                                                                                                                                                  |              |             |
|  **22**   | **x(n-3)={1 ; n=0 , 0 ; otherwise**                                                                                                                                                  |              |             |
|  **23**   | **x(n-3)={n ; n>0 , 0 ; n =< 0**                                                                                                                                                     |              |             |
|  **24**   | **x(n+4)={n ; n>0 , 0 ; n =< 0**                                                                                                                                                     |              |             |
|  **25**   | **x(n+3)={1 ; n>=0 , 0 ; n < 0**                                                                                                                                                     |              |             |
|  **26**   | **x(n-3)={1 ; n>=0 , 0 ; n < 0**                                                                                                                                                     |              |             |
|  **27**   | **x(n)={1 ; n=0 , 0 ; n ≠ 0**                                                                                                                                                        |              |             |
|  **28**   | **x(n-2)={1 ; n=2 , 0 ; n ≠ 2**                                                                                                                                                      |              |             |
|  **29**   | **x(n)={1 ; n >=0 , 0 ; n < 0**                                                                                                                                                      |              |             |
|  **30**   | **x(n-2) = {1 ; n >= 2 , 0 ; n < 2**                                                                                                                                                 |              |             |
|  **31**   | **x(n-2) = {n-2 ; n >= 2 , 0 ; n < 2**                                                                                                                                               |              |             |
|  **32**   | **Generating a sine wave**                                                                                                                                                           |              |             |
|  **33**   | **Generating a cosine wave**                                                                                                                                                         |              |             |
|  **34**   | **Generating a sine wave add to the cosine wave**                                                                                                                                    |              |             |
|  **35**   | **Sawtooth generates a sawtooth wave with peaks at +-1 and a period of 2π .An optional width parameter specifiers a fractional multiple of 2π at which the signals maximum occurs.** |              |             |
|  **36**   | **To generate 1.5s of a 50Hz sawtooth wave with a sample rate of 10kHz and plot 0.2s of the generate waveform.**                                                                     |              |             |
|  **37**   | **Generating Exponential signal.**                                                                                                                                                   |              |             |
|  **38**   | <p>**Generating a unit ramp.**</p><p></p>                                                                                                                                            |              |             |
|  **39**   | **Generates 40 samples of a unit step signal,u(n).**                                                                                                                                 |              |             |
|  **40**   | **Generating 64 samples of a unit impulse signal.**                                                                                                                                  |              |             |

**01.Experiment Name:Matlab code for Generation of unit impulse signal with delay and advance.**

**Matlab Code:**

**%Generation of unit impulse signal with delay and advance**

clc;

clf;

clear all;

close all;

N=20;

n=-N:1:N;

subplot(3,1,1);

x=[zeros(1,N) 1 zeros(1,N)];

stem(n,x);

grid;

title("Unit impulse signal");

xlabel("Discrete time ---N>>>");

ylabel("Amplitude");

subplot(3,1,2);

x=[zeros(1,N+5) 1 zeros(1,N-5)];

stem(n,x);

grid;

title("Unit impulse delay signal");

xlabel("Discrete time ---N>>>");

ylabel("Amplitude");

subplot(3,1,3);

x=[zeros(1,N-5) 1 zeros(1,N+5)];

stem(n,x);

grid;

title("Unit impulse advance signal");

xlabel("Discrete time ---N>>>");

ylabel("Amplitude");

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.002.png)

**02.Experiment Name:Matlab code for Generation of unit step signal with delay and advance.**

**Matlab Code:**

**%Generation of unit step signal with delay and advance**

clc;

clf;

clear all;

close all;

N=20;

n=-N:1:N;

subplot(3,1,1);

x=[zeros(1,N) 1 ones(1,N)];

stem(n,x);

grid;

title("Unit step signal");

xlabel("Discrete time ---N>>>");

ylabel("Amplitude");

subplot(3,1,2);

x=[zeros(1,N+5) 1 ones(1,N-5)];

stem(n,x);

grid;

title("Unit step delay signal");

xlabel("Discrete time ---N>>>");

ylabel("Amplitude");

subplot(3,1,3);

x=[zeros(1,N-5) 1 ones(1,N+5)];

stem(n,x);

grid;

title("Unit step advance signal");

xlabel("Discrete time ---N>>>");

ylabel("Amplitude");

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.003.png)

**03.Experiment Name:Matlab code for Generation of unit ramp signal with delay and advance.**

**Matlab Code:**

**%Generation of unit ramp signal with delay and advance**

clc;

clf;

clear all;

close all;

N=20;

n=-N:1:N;

subplot(3,1,1);

x=n.\*(n>=0);

stem(n,x);

grid;

title("Unit ramp signal");

xlabel("Discrete time ---N>>>");

ylabel("Amplitude");

subplot(3,1,2);

x=n.\*(n>=5);

stem(n,x);

grid;

title("Unit ramp delay signal");

xlabel("Discrete time ---N>>>");

ylabel("Amplitude");

subplot(3,1,3);

x=n.\*(n>=-5);

stem(n,x);

grid;

title("Unit ramp advance signal");

xlabel("Discrete time ---N>>>");

ylabel("Amplitude");

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.004.png)

**04.Experiment Name:y=sin(t).**

**Matlab Code:**

clc;

clf;

clear all;

close all;

` `t=-pi:(pi/16):pi;

y=sin(t);

` `plot(t,y);

` `hold on;

stem(t,y);

hold on;

` `plot(t,y);

grid;

` `title('sin wave');

xlabel('Continous time(t)');

` `ylabel('Amplitude')

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.005.png)

**05.Experiment Name:y=4\*sin(t)^2 , -2\*pi<t<2\*pi**

**Matlab Code:**

clc;

clf;

clear all;

close all;

t= -2\*pi:(pi/16):2\*pi;

y=4\*sin(t).^2;

plot(t,y);

hold on;

grid;

title('4\*sin(t)^2');

xlabel('Continous time(t)');

ylabel('Amplitude')

**Output:**

` `**![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.006.png)**

**06.Experiment Name:y=4\*sin(ωt)+cos(ωt) , -2\*pi<t<2\*pi**

**Matlab Code:**

clc;

clf;

clear all;

close all;

t=-2\*pi:(pi/5):2\*pi;

y=4\*sin(2\*pi\*5\*t)+cos(2\*pi\*5\*t);

plot(t,y);

hold on;

stem(t,y);

grid;

title('sin and cosine wave');

xlabel('Continous time(t)');

ylabel('Amplitude')

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.007.png)

**07.Experiment Name:y=cos(t)**

**Matlab Code:**

clc;

clf;

clear all;

close all;

t=-pi:(pi/5):2\*pi;

y=cos(t);

plot(t,y);

hold on;

stem(t,y);

grid;

title('cosine Wave');

xlabel('Continous time(t)');

ylabel('Amplitude')

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.008.png)

**08.Experiment Name:y=t==0 , -2\*pi<t<2\*pi**

**Matlab Code:**

clc;

clf;

clear all;

close all;

t=-2\*pi:(pi/5):2\*pi;

y=t==0;

plot(t,y);

hold on;

grid;

title('unit impulse signal');

xlabel('Continous time(t)');

ylabel('Amplitude')

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.009.png)

**09.Experiment Name:y=4\*cos(t)^2 , -2\*pi<t<2\*pi**

**Matlab Code:**

clc;

clf;

clear all;

close all;

t= -2\*pi:(pi/10):2\*pi;

y=4\*cos(t).^2;

plot(t,y);

hold on;

grid;

title('4\*cos(t)^2');

xlabel('Continous time(t)');

ylabel('Amplitude')

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.010.png)

**10.Experiment Name:step =t>=0 , t=-1:0.109:1**

**Matlab Code:**

clc;

clf;

clear all;

close all;

t=-1:0.109:1;

step=t>=0;

plot(t,step);

hold on;

stem(t,step);

grid;

title('Unit step');

xlabel('Continuous time(t)');

ylabel('Amplitude');

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.011.png)

**11.Experiment Name:y=t\*ramp , ramp=t>=0 , t=-1:0.1:1**

**Matlab Code:**

clc;

clf;

clear all;

close all;

t=-1:0.109:1;

ramp=t>=0;

y=t.\*ramp;

plot(t,y);

hold on;

stem(t,y);

grid;

title('Unit ramp');

xlabel('Continuous time(t)');

ylabel('Amplitude');

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.012.png)

**12.Experiment Name:When x(n)={1 ; n >= 0 , 0 ; n <0**

**Matlab Code:**

clc;

clf;

clear all;

close all;

n=-20:20;

x(n>=0)=1;

title('Straight line');

stem(n,x)

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.013.png)

**13.Experiment Name:x(n-2)={1 ; n>=0 , 0 ; n<0**

**Matlab Code:**

clc;

clf;

clear all;

close all;

n=-20:20;

x((n-2)>=0)=1;

stem(n,x);

title('Straight line');

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.014.png)

**14.Experiment Name:x(n+2)={1 ; n>=0 , 0 ; n<0**

**Matlab Code:**

clc;

clf;

clear all;

close all;

n=-20:20;

x((n+2)>=0)=1;

stem(n,x);

title('Straight line');

xlabel('n');

ylabel('x');

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.015.png)

**15.Experiment Name:x(n)={n ; n>0 , 0 ; n=<0**

**Matlab Code:**

clc;

clf;

clear all;

close all;

n=-20:20;

x=n.\*(n>0);

stem(n,x);

title('Mid line');

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.016.png)

**16.Experiment Name:x(n-2)={n ; n>0 , 0 ; n=<0**

**Matlab Code:**

clc;

clf;

clear all;

close all;

n=-20:20;

x=n.\*((n-2)>0);

stem(n,x);

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.017.png)

**17.Experiment Name:x(n+2)={n ; n>0 , 0 ; n=<0**

**Matlab Code:**

clc;

clf;

clear all;

close all;

n=-20:20;

x=n.\*((n+2)>0);

stem(n,x);

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.018.png)

**18.Experiment Name:x(n)={1 ; n=0 , 0 ; otherwise**

**Matlab Code:**

clc;

clf;

clear all;

close all;

n=-20:20;

N=40;

x=[zeros(1,(N/2)),1,zeros(1,(N/2))];

stem(n,x);

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.019.png)

**19.Experiment Name:x(n-5)={1 ; n=0 , 0 ; otherwise**

**Matlab Code:**

clc;

clf;

clear all;

close all;

n=-20:20;

N=40;

x=[zeros(1,(N/2-5)),1,zeros(1,(N/2+5))];

stem(n,x);

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.020.png)

**20.Experiment Name:x(n+5)={1 ; n=0 , 0 ; otherwise**

**Matlab Code:**

clc;

clf;

clear all;

close all;

n=-20:20;

N=40;

x=[zeros(1,(N/2+5)),1,zeros(1,(N/2-5))];

stem(n,x);

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.021.png)

**21.Experiment Name:x(n+8)={1 ; n=0 , 0 ; otherwise**

**Matlab Code:**

clc;

clf;

clear all;

close all;

n=-20:20;

N=40;

x=[zeros(1,(N/2+8)),1,zeros(1,(N/2-8))];

stem(n,x);

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.022.png)

**22.Experiment Name:x(n-3)={1 ; n=0 , 0 ; otherwise**

**Matlab Code:**

clc;

clf;

clear all;

close all;

n=-20:20;

N=40;

x=[zeros(1,(N/2-3)),1,zeros(1,(N/2+3))];

stem(n,x);

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.023.png)

**23.Experiment Name:x(n-3)={n ; n>0 , 0 ; n =< 0**

**Matlab Code:**

clc;

clf;

clear all;

close all;

n=-20:20;

x=n.\*((n-3)>0);

stem(n,x);

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.024.png)

**24.Experiment Name:x(n+4)={n ; n>0 , 0 ; n =< 0**

**Matlab Code:**

clc;

clf;

clear all;

close all;

n=-20:20;

x=n.\*((n+4)>0);

stem(n,x);

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.025.png)

**25.Experiment Name:x(n+3)={1 ; n>=0 , 0 ; n < 0**

**Matlab Code:**

clc;

clf;

clear all;

close all;

n=-20:20;

x((n+3)>=0)=1;

stem(n,x);

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.026.png)

**26.Experiment Name:x(n-3)={1 ; n>=0 , 0 ; n < 0**

**Matlab Code:**

clc;

clf;

clear all;

close all;

n=-20:20;

x((n-3)>=0)=1;

stem(n,x);

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.027.png)

**27.Experiment Name:x(n)={1 ; n=0 , 0 ; n ≠ 0**

**Matlab Code:**

clc;

clf;

clear all;

close all;

n=-5:5;

x=(n==0);

stem(n,x);

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.028.png)

**28.Experiment Name:x(n-2)={1 ; n=2 , 0 ; n ≠ 2**

**Matlab Code:**

clc;

clf;

clear all;

close all;

n=-5:5;

x=((n-2)==0);

stem(n,x);

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.029.png)

**29.Experiment Name:x(n)={1 ; n >=0 , 0 ; n < 0**

**Matlab Code:**

clc;

clf;

clear all;

close all;

n=-5:5;

x=(n>=0);

stem(n,x);

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.030.png)

**30.Experiment Name:x(n-2) = {1 ; n >= 2 , 0 ; n < 2**

**Matlab Code:**

clc;

clf;

clear all;

close all;

n=-5:5;

x=((n-2)>=0);

stem(n,x);

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.031.png)

**31.Experiment Name:x(n-2) = {n-2 ; n >= 2 , 0 ; n < 2**

**Matlab Code:**

clc;

clf;

clear all;

close all;

n=-20:20;

x=(n-2).\*((n-2)>=0);

stem(n,x);

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.032.png)

**32.Experiment Name:Generating a sine wave**

**Matlab Code:**

**%continous sinewave**

clc;

clf;

clear all;

close all;

t=0:0.1:10;

y=2\*sin(2\*pi\*0.5\*t);

plot(t,y)

title("continous sinewave");

xlabel("time");

ylabel("amplitude");

grid on;

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.033.png)

**33.Experiment Name:Generating a cosine wave**

**Matlab Code:**

**%continous cosinewave**

clc;

clf;

clear all;

close all;

t=0:0.1:10;

y=2\*cos(2\*pi\*0.5\*t);

plot(t,y)

title("continous cosinewave");

xlabel("time");

ylabel("amplitude");

grid on;

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.034.png)

**34.Experiment Name:Generating a sine wave add to the cosine wave**

**Matlab Code:**

**%continous sinewave**

clc;

clf;

clear all;

close all;

t=0:0.1:10;

y=2\*sin(2\*pi\*0.5\*t);

plot(t,y,'r');

hold on;

%continous cosinewave

t=0:0.1:10;

y=2\*cos(2\*pi\*0.5\*t);

plot(t,y,'b');

xlabel("time");

ylabel("amplitude");

grid on;

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.035.png)

**35.Experiment Name:Sawtooth generates a sawtooth wave with peaks at +-1 and a period of 2π .An optional width parameter specifiers a fractional multiple of 2π at which the signals maximum occurs.**

**Matlab Code:**

**%sawtooth wave**

clc;

clf;

clear all;

close all;

t=0:0.1:30;

x=sawtooth(t);

plot(t,x)

title(" Sawtooth wave");

xlabel("Time index");

ylabel("Amplitude");

grid on;

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.036.png)

**36.Experiment Name:o generate 1.5s of a 50Hz sawtooth wave with a sample rate of 10kHz and plot 0.2s of the generate waveform.**

**Matlab Code:**

clc;

clf;

close all;

clear all;

fs = 10000;

t = 0:1/fs:1.5;

x = sawtooth(2\*pi\*50\*t);

plot(t,x),axis([0 0.2 -1.2 1.2]);

xlabel('Time index');

ylabel('Amplitude');

title('50 Hz sawtooth wave');

grid;

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.037.png)

**37.Experiment Name:Generating Exponential signal.**

**Matlab Code:**

**%Generate Exponential signal x(t)=exp(-1\*t)**

clc;

clf;

clear all;

close all;

t=0:0.1:40;

x=exp(-0.1\*t);

plot(t,x);

grid;

title("Exponential Signal");

xlabel("Time Index[ms]");

ylabel("Amplitude");

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.038.png)

**38.Experiment Name:Generating a unit ramp.**

**Matlab Code:**

**%Generate a unit ramp**

clc;

clf;

clear all;

close all;

t=-1:0.01:1;

r=t.\*(t>=0);

plot(t,r);

grid;

title("Unit ramp");

xlabel("t");

ylabel("r");

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.039.png)

**39.Experiment Name:Generates 40 samples of a unit step signal,u(n).**

**Matlab Code:**

clc;

clf;

clear all;

close all;

N=40;

n=-20:20;

u=[zeros(1,(N/2)+1),ones(1,(N/2))];

plot(n,u);

grid;

title("A unit step signal");

xlabel("Sample Numbers");

ylabel("Amplitude");

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.040.png)

**40.Experiment Name:Generating 64 samples of a unit impulse signal.**

**Matlab Code:**

clc;

clf;

clear all;

close all;

N=64;

n=-(N/2):((N/2)-1);

x=zeros(1,N);

x((N/2)+1)=1.0;

plot(n,x);

grid;

title("A unit impulse signal");

xlabel("Sample Numbers");

ylabel("Amplitude");

**Output:**

![](Aspose.Words.91d2d51d-3a14-4799-a1ec-351be8d9bb48.041.png)
