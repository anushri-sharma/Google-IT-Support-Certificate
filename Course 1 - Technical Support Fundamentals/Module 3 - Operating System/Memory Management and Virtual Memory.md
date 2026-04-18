[Memory Management and Virtual Memory](https://www.youtube.com/watch?v=vpHXJb89qZA)

Remember that when a process runs, it needs CPU time, but it also needs memory.

When processes are run, they have to take up space in memory, so that the computer can read and load them quickly.

However, compared to our hard disk drives, memory comes in smaller quantities.

So to give us more memory than we physically have, we use something called **virtual memory**.

<img width="1277" height="441" alt="image" src="https://github.com/user-attachments/assets/d9d8b333-9510-41b4-bc02-9b71a51d8fe9" />

**Virtual memory is the combination of hard drive space and RAM that acts like memory that our processes can use**.

When we execute a process, we take the data of the program in chunks we call **pages**.

**We store these pages in virtual memory.**

<img width="1273" height="690" alt="image" src="https://github.com/user-attachments/assets/672fbe44-5924-4312-913b-55360706182f" />

If we want to read and execute these pages, they have to be sent to physical memory or RAM.

Why don't we just store the entire program in RAM so we can execute it quickly?

Well you could, if it was small enough, but for large applications it would be wasteful.

Have you ever worked in a word processor and then gone to a menu don't normally use and noticed the application slow down a little?

It's because your computer had to load the page for that menu from virtual memory into RAM.

We don't use all the features of our application at once.

So why load it up at once?

It's similar to cooking a recipe from a cookbook.
You don't need to read the whole book just to make one recipe.
You only need to read the pages of the recipe you're currently using.

When we **store** our **virtual memory** on our **hard drive**, we call the allocated space **swap space**.

When we get into practical applications of disk partitioning, **we'll allocate space for swap**.

The **kernel** takes care of all of this for us of course.

**It handles the process of taking pages of data and swapping them between RAM and virtual memory**.\

01:39
But, the kernel isn't the only hard worker around.
