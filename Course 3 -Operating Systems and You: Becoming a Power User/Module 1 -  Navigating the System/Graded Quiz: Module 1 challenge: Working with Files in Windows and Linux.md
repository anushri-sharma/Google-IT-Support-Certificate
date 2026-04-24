
# Graded Quiz: Module 1 challenge: Working with Files in Windows and Linux

<img width="705" height="404" alt="image" src="https://github.com/user-attachments/assets/0428f184-daf4-4c03-9ed1-6bc9b0c3029a" />

```
Why:

- This option enables Windows File Explorer to look inside files (file contents)
in addition to just searching by filename.

Why others are incorrect:

- Search all files → Not a specific option for content search
- Include system directories → Expands search locations, not content
- Include compressed files → Allows searching inside ZIP files, not general file contents

✔️ Final answer: Always search file names and contents
```

<img width="772" height="548" alt="image" src="https://github.com/user-attachments/assets/20329e7f-f91d-4d7c-8205-16138ea68ce6" />

<img width="701" height="455" alt="image" src="https://github.com/user-attachments/assets/76173335-2f05-40de-9e4b-89f7f916f315" />

<img width="681" height="381" alt="image" src="https://github.com/user-attachments/assets/16d35bfd-aab5-486a-ac4f-5d50641cdb00" />

```
✅ Correct answer:
cp documents C:\Users\old -Recurse


Why this is correct:
- cp (alias for Copy-Item in PowerShell) copies files/folders
- documents → source folder (inside C:\Users)
- C:\Users\old → destination

### -Recurse → ensures all contents (files + subfolders) are copied

Why others are incorrect:

- cp documents C:\Users\old → ❌ misses -Recurse, so contents won’t copy properly

- cp documents C:\Users\old\documents -Recurse -Verbose → ⚠️ works but unnecessarily
specifies a new folder name (not required in this question)

- cp documents C:\Users\old\documents → ❌ missing -Recurse



```

<img width="836" height="607" alt="image" src="https://github.com/user-attachments/assets/f6863f66-4f26-4932-a6ba-5ec60f524757" />

<img width="682" height="390" alt="image" src="https://github.com/user-attachments/assets/e4969f0f-29c2-4c87-ada3-0e728ec3f63e" />

<img width="764" height="437" alt="image" src="https://github.com/user-attachments/assets/be17d632-ed2b-47cb-bbb1-9fb79834452f" />

```
Why these work:
cd C:\Users\pictures\dogs
   → Uses an absolute path, so it directly takes you to the dogs folder from anywhere.
cd ..\dogs
   → .. moves up one level (from cats → pictures), then enters dogs → correct relative path.

❌ Why the others are incorrect:

cd ~\cats ~\dogs
   → Invalid syntax; you can’t pass multiple paths like this.
cd ~\dogs
   → ~ refers to the user’s home directory (C:\Users\YourName), not C:\Users\pictures,
     so this path is incorrect.

```

<img width="748" height="475" alt="image" src="https://github.com/user-attachments/assets/9f6648f6-0614-40cf-aaa7-4333db3834f1" />

<img width="703" height="412" alt="image" src="https://github.com/user-attachments/assets/95a0a60a-a6c7-4492-a7e4-2ccef5c77ddf" />

```
PWD - Prints the present working directory.
```

<img width="736" height="476" alt="image" src="https://github.com/user-attachments/assets/d4398b0b-004b-4a30-8c18-c2b4baa83835" />
