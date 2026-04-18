# Practice Quiz: Binary

<img width="759" height="423" alt="image" src="https://github.com/user-attachments/assets/18558cce-a613-4b66-a5bd-4615a8f35b13" />

```
To convert 45 into binary using the table:
128  64  32  16  8  4  2  1
We break 45 into powers of 2:
45 = 32 + 8 + 4 + 1
Now mark the table:
128 → 0
64 → 0
32 → 1
16 → 0
8 → 1
4 → 1
2 → 0
1 → 1
So the binary form is:
00101101
✅ Correct answer: 00101101

```


<img width="737" height="401" alt="image" src="https://github.com/user-attachments/assets/18edb815-253d-4b41-8f5e-d445da834fe6" />

```
An 8-bit byte can represent 2⁸ different values.
That is:
2⁸ = 256
✅ Correct answer: 256

```


<img width="740" height="403" alt="image" src="https://github.com/user-attachments/assets/6f9842b3-9f45-4b80-9719-f3ae9e5ca99f" />

```
A byte has 8 bits, so it can represent values from:
0 (all bits 0: 00000000)
to 255 (all bits 1: 11111111)
That’s a total of 256 values, but since counting starts at 0, the highest decimal value is:
✅ 255

```


<img width="823" height="484" alt="image" src="https://github.com/user-attachments/assets/a98aa0f5-6cfc-4fa9-af66-8e3a108b49f4" />

```
Using the binary table:
128  64  32  16   8   4   2   1
 1    0    1    0   1   0   1   0
Add the positions where there is 1:
128 + 32 + 8 + 2 = 170
✅ Correct answer: 170

```

<img width="784" height="417" alt="image" src="https://github.com/user-attachments/assets/7840a45c-2550-416c-bba1-6314e6adc5ff" />

```
ASCII is limited to 128 characters (basic English letters, numbers, and symbols),
which isn’t enough for global languages or modern symbols.
UTF-8 replaced it because:
✅ UTF-8 can store a character in more than one byte.
This allows it to represent millions of characters, including different languages and emojis,
while still being compatible with ASCII for basic text.

```

🔹 1. What Binary Is

The video explains that computers don’t understand decimal numbers (0–9).

Instead, they use binary (base-2 system):

Only two digits: 0 and 1

These digits are called bits.

👉 Key idea:

Everything in a computer—text, images, videos—is ultimately stored as binary code.

🔹 2. Understanding Bit Positions (Binary Table)

The video introduces a table like:

128  64  32  16  8  4  2  1

Each position represents a power of 2

From right to left:

2⁰, 2¹, 2², 2³ … up to 2⁷

👉 This table is used to:

Convert binary → decimal

Convert decimal → binary

🔹 3. Binary to Decimal Conversion

The method shown:

Write the binary number under the table

Add values where there is 1

Example (like in video):

10101010

= 128 + 32 + 8 + 2

= 170

👉 Key rule:

Only add positions where the bit = 1

🔹 4. Decimal to Binary Conversion

The reverse process:

Break the decimal number into powers of 2

Example:

45 = 32 + 8 + 4 + 1

Then fill the table:

00101101

🔹 5. What is a Byte

A byte = 8 bits

This is a standard unit in computing

👉 Important range:

Minimum: 00000000 → 0

Maximum: 11111111 → 255

So:

Total values = 256 (0–255)

🔹 6. Why Binary Matters

The video explains:

Computers use electrical signals:

ON → 1

OFF → 0

Binary is simple and reliable for hardware

🔹 7. Character Encoding (ASCII → UTF-8)

Older systems used ASCII (limited to 128 characters)

Modern systems use UTF-8

Supports multiple languages and emojis

Uses more than one byte when needed

🔹 8. Practice & Application

The video includes:

Practice problems

Step-by-step solving

Reinforcement of:

Binary conversions

Byte limits

Real-world usage

✅ Key Takeaways

Binary uses only 0 and 1

Each position = power of 2

**8 bits = 1 byte**

Max value of a byte = 255

Binary is the foundation of all computing systems

📌 Simple One-Line Summary

👉 The video teaches how computers use binary (0s and 1s) to represent data and shows how to convert between binary and decimal using powers of 2.


