
[Abstraction](https://www.youtube.com/watch?v=9iKFp1FOujE&t=2s)

🔥 **How a CPU executes instructions**
  – **Binary code (bits)** is sent to a **CPU**, and the CPU uses an **instruction set** to execute those commands.

<img width="1267" height="539" alt="image" src="https://github.com/user-attachments/assets/764f5bdb-6f3b-4c8d-8139-7fcdd4bed44e" />

<img width="1274" height="631" alt="image" src="https://github.com/user-attachments/assets/be1f2273-4b5e-4e06-80be-e67034bca626" />

<img width="1268" height="423" alt="image" src="https://github.com/user-attachments/assets/a821b0ae-5de7-4e22-8cad-469492289797" />

🍳 **Hardware diversity and differing interfaces**
  – CPUs from different manufacturers can have **different instruction sets**.
  – Other hardware components (for example, **video cards** and **hard drives**) expose their own **special interfaces**.

💡 **The naive approach and its infeasibility**
  – One could write a separate program for each possible CPU and hardware combination using their **native languages and interfaces**.
  – This is impractical because there are potentially **millions of possible configurations** of hardware.

🧩 **Role of computer science and abstraction**
  – Through the efforts of computer scientists and the **principle of abstraction**, higher-level solutions were developed to hide hardware differences.
  – Abstraction provides layers that present uniform interfaces above diverse hardware specifics.

🔧 **Programming languages as the practical solution**
  – **Programming languages** let developers write instructions at a higher level rather than in hardware-specific binary or native interfaces.
  – These languages, together with the abstraction layers beneath them, enable programs to be **run on many different hardware configurations**.

📌 **Implication for software portability**
  – Abstraction reduces the need to target every hardware variant directly, making software **more portable** across different CPUs and peripherals.
