# Intro to computers 

<img width="1164" height="360" alt="image" src="https://github.com/user-attachments/assets/19513169-0fa7-4d99-a6b2-ee6903bd3ea4" />

<img width="1276" height="319" alt="image" src="https://github.com/user-attachments/assets/5a47c326-c568-4321-9921-b61895539868" />

<img width="1280" height="328" alt="image" src="https://github.com/user-attachments/assets/403a6a88-0a49-4cf6-97ad-52e4edd180ef" />

<img width="1277" height="354" alt="image" src="https://github.com/user-attachments/assets/6f197262-2cdc-42e5-8894-ef31d5b86695" />

<img width="1276" height="362" alt="image" src="https://github.com/user-attachments/assets/40a985df-e47e-4590-a2e7-a16b33f8540f" />

<img width="1280" height="282" alt="image" src="https://github.com/user-attachments/assets/9799feb1-9f3d-4b63-ae6b-377934b59603" />

<img width="1276" height="298" alt="image" src="https://github.com/user-attachments/assets/c22674ae-f49a-43a0-8dd9-4451d15397c5" />

<img width="1273" height="418" alt="image" src="https://github.com/user-attachments/assets/a9de4878-d6f1-4f1c-b5af-5be4d5281bd3" />

<img width="1277" height="321" alt="image" src="https://github.com/user-attachments/assets/e6aabf80-a068-4cf7-a8b8-84eb45149621" />

<img width="1280" height="349" alt="image" src="https://github.com/user-attachments/assets/9a3cead2-d7ad-49da-bfb3-55d1daccc390" />

<img width="1279" height="382" alt="image" src="https://github.com/user-attachments/assets/31ae24e7-7c5b-456e-8538-9d007ad72672" />

<img width="1278" height="342" alt="image" src="https://github.com/user-attachments/assets/d5f51a1b-4544-4d4c-9ff5-2a5f3539000e" />

<img width="647" height="208" alt="image" src="https://github.com/user-attachments/assets/313830e9-8461-42ef-b6f2-6d45fd971af7" />

<img width="1280" height="357" alt="image" src="https://github.com/user-attachments/assets/6383ee8c-3c6c-42e2-97e9-ff6e80b824fd" />

<img width="530" height="270" alt="image" src="https://github.com/user-attachments/assets/4ef7e1cd-a08e-4a95-bd5c-57860d99487f" />

<img width="1272" height="298" alt="image" src="https://github.com/user-attachments/assets/2f95ab0e-c950-4bf8-9259-9adfe589353b" />

💡 Character encoding: what and why  
  – **Character encoding** is a mapping (like a dictionary) that assigns binary values to human-readable characters so computers can store and display text instead of raw zeros and ones.  
  – A **byte = 8 bits**, giving **256** possible distinct values per byte; encodings decide how those values map to characters.  

🔤 ASCII: the original standard  
  – **ASCII** is a **7-bit** encoding providing **128** values for the English alphabet, digits, and common punctuation.  
  – Example: lowercase **'a' = 01100001** in binary (decimal 97).  
  – ASCII was compact and sufficient for basic English text but lacked symbols and characters for many other languages.

🌐 Unicode and UTF‑8: scale and compatibility  
  – **Unicode** is a universal character repertoire designed to give unique code points to characters across scripts, symbols, and emojis.  
  – **UTF‑8** is a variable-length encoding of Unicode and the most widely used text encoding today.  
  – UTF‑8 is **backward compatible with ASCII**: ASCII characters use a single byte (same values as ASCII).  
  – UTF‑8 uses **1–4 bytes per character**, allowing representation of the large number of Unicode code points (including emojis) that cannot fit in a single byte.

🔣 Why variable-length encodings matter  
  – Many characters (for example, emojis, scripts beyond basic Latin) exceed **256** possibilities, so single-byte encodings are insufficient.  
  – Variable-length encodings let common characters remain compact (1 byte) while allowing rare/large-code-point characters to occupy multiple bytes.  
  – Proper encoding rules (like UTF‑8’s byte-prefix design) enable reliable decoding and resynchronization when reading streams of bytes.

🌍 Historical and practical implications  
  – Multiple legacy encodings were created to support different languages and symbol sets; this fragmentation caused interoperability issues.  
  – Unicode + UTF‑8 unified representation across languages and platforms, reducing the need for many different encodings.

🎨 Representing color in computers (RGB model)  
  – Color is represented with models such as **RGB (red, green, blue)**, where each pixel’s color is a combination of three channels.  
  – Common implementation uses **three channels**, each typically **8 bits** (one byte), giving **256 shades per channel**.  
  – Combined as **24‑bit color**, this yields about **16.7 million** distinct colors for each pixel.

🔢 Key numerical takeaways  
  – **1 byte = 8 bits → 256** possible values.  
  – **ASCII = 7 bits → 128** values (covers basic English letters, digits, punctuation).  
  – **UTF‑8 = 1–4 bytes per character** (supports full Unicode, including emojis).  
  – **RGB with 8 bits per channel = 24 bits → ~16.7 million colors**.

🔎 Practical example and summary linkages  
  – Single-byte encodings can represent simple English text (ASCII) but not global scripts or emojis.  
  – UTF‑8 preserves single-byte efficiency for ASCII while enabling multi-byte sequences for the wider Unicode set.  
  – The same underlying binary principle (bits and bytes) is used to represent both text and color on screens.
