
<img width="350" height="643" alt="image" src="https://github.com/user-attachments/assets/59694bba-fb40-40e3-86a5-133e5144f363" />


<img width="1280" height="409" alt="image" src="https://github.com/user-attachments/assets/5cd802c1-05f1-4d6b-85b8-5762a4db2060" />


<img width="1280" height="384" alt="image" src="https://github.com/user-attachments/assets/28d8eaee-679b-4e84-ab33-99800b817ae1" />


<img width="1278" height="396" alt="image" src="https://github.com/user-attachments/assets/ba733c82-4800-4f36-a12a-b47282d59744" />


<img width="1280" height="381" alt="image" src="https://github.com/user-attachments/assets/826b84e4-dcc4-4d50-a367-7ec7dc8dde9e" />


<img width="1279" height="406" alt="image" src="https://github.com/user-attachments/assets/f698efd9-cf50-433c-b7f6-4cb5532804f1" />


<img width="1271" height="416" alt="image" src="https://github.com/user-attachments/assets/da9ccb80-0845-4a4e-955a-164e1e82c895" />


<img width="1279" height="385" alt="image" src="https://github.com/user-attachments/assets/dd838060-8e14-4021-af46-998042337d66" />


<img width="1170" height="618" alt="image" src="https://github.com/user-attachments/assets/b55111d8-f782-4712-a6c3-6e0551611413" />


<img width="1206" height="587" alt="image" src="https://github.com/user-attachments/assets/5d6e75c9-1e4a-4c6d-a5e5-f329b6a1a8aa" />


<img width="1279" height="326" alt="image" src="https://github.com/user-attachments/assets/c5fc2d79-3bb7-4819-9ff9-425bd1381bc3" />


<img width="1267" height="385" alt="image" src="https://github.com/user-attachments/assets/33f71b42-a9b5-4706-acb6-895fafdfb8cb" />


<img width="1277" height="468" alt="image" src="https://github.com/user-attachments/assets/3fa9d521-bd9a-49b7-931a-4116927913f0" />


<img width="1278" height="336" alt="image" src="https://github.com/user-attachments/assets/9cedb922-bc19-4442-af7c-6ef7a6c15acb" />

🔢 **Binary communication and machine language**  
  - Computers communicate only in **1's and 0's**; human languages require a translation to this form, i.e., **machine language**.  
  - Instructions given to a computer must be converted into binary for the CPU to execute.

📁 **Programs and durable storage**  
  - **Programs** are sequences of instructions (analogous to recipes) that tell a computer what to do.  
  - Programs are typically stored on durable media such as **hard drives** (the "cookbook").

🍳 **CPU as the processor (“chef”)**  
  - The **CPU** executes program instructions; faster CPUs process more instructions per time, analogous to a faster chef making more food.  
  - CPUs operate on instructions one line at a time and require those instructions in binary form.

🧠 **RAM: short-term memory (copy of recipes)**  
  - Programs are copied from durable storage into **RAM** so the CPU can access instructions faster than reading from disk.  
  - **RAM** is randomly accessible memory—any location can be read as quickly as any other.  
  - Because RAM can hold millions or billions of entries, the CPU does not send entire programs across at once; it requests specific instructions as needed.

🔌 **How binary travels: buses and bit widths**  
  - The **external data bus (EDB)** is a set of wires that carries bits (voltages) between components; a wire with voltage = 1, without = 0.  
  - Buses come in widths like **8-bit, 16-bit, 32-bit, 64-bit**; wider buses move more data per transfer.  
  - Examples in the lesson use an **8-bit** EDB (one byte at a time).

🧾 **Registers inside the CPU**  
  - **Registers** are small storage locations inside the CPU used to hold operands and results (analogy: the chef’s work tables).  
  - Example: one value in **register A**, another in **register B**, result in **register C** when performing an addition.

🧭 **Memory Controller (MCC) and how data is fetched**  
  - The **memory controller chip (MCC)** bridges the CPU and RAM; the CPU requests a specific instruction or data item by index.  
  - The CPU sends the **location** over the **address bus** (address only, not the data); the MCC reads RAM at that address and sends the requested data over the **EDB** back to the CPU.  
  - This fetch cycle allows the CPU to handle instructions out of sequential order and avoids sending the entire program over the EDB.

📦 **Cache: faster, smaller memory close to the CPU**  
  - **Cache** is smaller but faster than RAM and stores recently or frequently used data for quick reference (analogy: pockets vs refrigerator).  
  - Typical cache hierarchy: **L1** (smallest, fastest), **L2**, **L3** (larger, slower than L1/L2 but faster than RAM).  
  - CPUs check cache before going to RAM to reduce latency.

⏱️ **CPU clock, cycles, and speed metrics**  
  - The CPU uses an internal **clock** connected to a **clock wire**; each tick is a **clock cycle** during which the CPU performs part or all of an operation.  
  - **Clock speed** is the number of cycles per second; e.g., **3.4 GHz = 3.4 billion cycles per second** represents the maximum cycle rate.  
  - Real performance depends on work per cycle, memory/cache performance, and other factors; clock speed is an upper bound for cycles per second.

⚠️ **Overclocking: increasing clock rate and risks**  
  - **Overclocking** raises the CPU clock rate above its nominal specification to increase performance (common in gaming/low-end CPU tuning).  
  - Risks include increased heat generation and potential instability or hardware damage if not properly cooled or configured.
