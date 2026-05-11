# Practice Quiz: How to Count in Binary

<img width="606" height="327" alt="image" src="https://github.com/user-attachments/assets/51feb8d1-c503-48e3-a7ae-c76672aee4df" />

```
88 = 64 + 16 + 8
Binary = 1011000 ✅ (correct)
```

<img width="677" height="349" alt="image" src="https://github.com/user-attachments/assets/1845a68c-a52c-466e-b566-36c2ca6d0b6f" />

```
To represent "code" in binary, we use ASCII values for each character:
c → 01100011
o → 01101111
d → 01100100
e → 01100101
✅ Correct Answer:
01100011 01101111 01100100 01100101
```

<img width="637" height="315" alt="image" src="https://github.com/user-attachments/assets/5dcad208-fc92-4256-8016-b1266c1bf3af" />

```
245 = 128 + 64 + 32 + 16 + 4 + 1
Binary = 11110101 ✅ (correct)
```

<img width="739" height="365" alt="image" src="https://github.com/user-attachments/assets/2e8541da-334e-429d-a477-bc21dc7ac650" />

```
Convert 01110100 from binary to decimal using place values:
128  64  32  16   8   4   2   1
 0    1    1    1   0   1   0   0
Add the positions with 1:
64 + 32 + 16 + 4 = 116
```

<img width="657" height="326" alt="image" src="https://github.com/user-attachments/assets/ca5e7bc1-1bb4-4f90-8e09-cd4c628a7645" />

```
215 = 128 + 64 + 16 + 4 + 2 + 1
Binary = 11010111 ✅ (correct)
```

<img width="702" height="366" alt="image" src="https://github.com/user-attachments/assets/0b464ad8-66dc-4b23-bc43-0d1f1e0a5efa" />

```
Convert 01001101 using the binary table:
128  64  32  16   8   4   2   1
 0    1    0    0   1   1   0   1
Add the values where there is 1:
64 + 8 + 4 + 1 = 77
```

<img width="716" height="336" alt="image" src="https://github.com/user-attachments/assets/b998d403-d7e6-4252-a593-3d45f546f592" />

```
Convert each character using ASCII:
h → 01101000
i → 01101001
✅ Correct Answer:
01101000 01101001
```

## How to Count in Binary

<br>

### Question 1

In this activity, you will use the tool below to help you convert a decimal number into binary form. When a 1 is used, we consider the value to be “ON.” When a 0 is used, we consider the value to be “OFF.”

Click the binary bits necessary to compute the decimal value on the right column. You have 10 calculations to complete.

![img](binary-calculator.png)

<br>

### Some usefull script

```
>>> decimals = [82,117,66,55,102,51,84,62,5,57] # change value
>>> for num in decimals:
...     print(f"{num}: {format(num, '08b')}")
... 
82: 01010010
117: 01110101
66: 01000010
55: 00110111
102: 01100110
51: 00110011
84: 01010100
62: 00111110
5: 00000101
57: 00111001
```
