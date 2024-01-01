# command-line-arguments-to-count-word
## AIM:
To write a python program for getting the word count from the contents of a file using command line arguments.
## EQUIPEMENT'S REQUIRED: 
PC
Anaconda - Python 3.7
## ALGORITHM: 
## Step 1:
Import the sys module.

## Step 2:
Pass the filename as the first argument after the name of script. Open the file as sys.argv[1]

## Step 3:
Read the file using read() method.

## Step 4:
Use split() method to split the file content into words.

## Step 5:
Use len() to find the total words.

## Step 6:
Use len() to find the total words.

## PROGRAM:
```
#Program for getting word count from the contents of a file using command line arguments.
#Developed by: guntur shaik mohammad shahil
#Reg No: 212223240044

import sys
count={}
with open(sys.argv[1],'r') as f:
    for line in f:
        for word in line.split():
            if word not in count:
                count[word]=1
            else:
                count[word]+=1
print(count)
f.close()
```
### OUTPUT:
![image](https://github.com/22002102/command-line-arguments-to-count-word/assets/119091638/bfcbf15c-adab-4f9a-89a3-92aa071c69d0)
![image](https://github.com/22002102/command-line-arguments-to-count-word/assets/119091638/6749630c-d6ae-47fd-b1b3-e18dcf403ff8)


## RESULT:
Thus the program is written to find the word count from the contents of a file using command line arguments.
