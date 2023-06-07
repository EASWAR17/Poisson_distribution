# Fitting Poisson  distribution
# Aim : 

To fit poisson distribution for the arrival of objects per minute from the feeder

# Software required :  

Python and Visual component tool

# Theory:

The Poisson distribution is the discrete probability distribution of the number of events occurring in a given time period, given the average number of times the event occurs over that time period.

![image](https://user-images.githubusercontent.com/104613195/166248326-fd042076-8b0b-40c4-8b11-1d8e8fcb74db.png)

 Conditions for Poisson Distribution:

1. An event can occur any number of times during a time period.
2. Events occur independently. I
3. The rate of occurrence is constant.
4. The probability of an event occurring is proportional to the length of the time period. 
 
# Procedure :

![image](https://user-images.githubusercontent.com/104613195/166251988-d0c53205-6080-4f7b-ae4c-398178586637.png)

# Experiment :

![image](https://user-images.githubusercontent.com/103921593/230282876-f4a5afbf-cac1-4648-a1b0-c78840638a8e.png)

# Program :
```
import numpy as np
import math
import scipy.stats

L=[int(i) for i in input().split()]
N=len(L)
M=max(L)
x=list()
f=list()
for i in range (M+1):
    c=0
    for j in range(N):
        if L[j]==i:
            c=c+1
    f.append(c);
    x.append(i)
print(x)
print(f)
```
 

# Output : 

## input, x and x occurance list
![image](https://github.com/EASWAR17/Poisson_distribution/assets/94154683/53781f53-101c-4ca0-ba7f-a5f99fafbdb2)

## sum of occurences
![image](https://github.com/EASWAR17/Poisson_distribution/assets/94154683/e0b4455f-7218-4f9d-8087-fa6b2566ceb9)


## probability list
![image](https://github.com/EASWAR17/Poisson_distribution/assets/94154683/3f3e087f-5a18-4de0-a87f-5b94908fe343)

## Poisson Distribution Table
![image](https://github.com/EASWAR17/Poisson_distribution/assets/94154683/a8af39c7-e4bf-40ff-851e-398b342b5bbe)

## precision metrics
![image](https://github.com/EASWAR17/Poisson_distribution/assets/94154683/2b3d3709-87ab-425a-897d-3e9f33489c0c)

# Results

The Poisson distribution is fitted for the objects arrived from feeder per minute and the data is tested using Chi-square test. 
 
