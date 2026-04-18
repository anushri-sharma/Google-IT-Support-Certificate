# Process Management


[Process Management](https://www.youtube.com/watch?v=Q0ZTMoHemEY)

<img width="1279" height="361" alt="image" src="https://github.com/user-attachments/assets/5edcb3e6-0146-4d1e-8371-7fbcab5cf4fc" />


<img width="1270" height="377" alt="image" src="https://github.com/user-attachments/assets/adaffaef-f73e-4562-9dff-54d79cd30f51" />


<img width="1272" height="714" alt="image" src="https://github.com/user-attachments/assets/57cafbc3-dcef-4445-a62e-4a1f33ef0cd8" />


<img width="1280" height="398" alt="image" src="https://github.com/user-attachments/assets/4d7fdc8a-65f7-46bf-a13f-7c3ce8cf2a4f" />


<img width="1280" height="404" alt="image" src="https://github.com/user-attachments/assets/d31f9388-15e4-45d2-bf94-a8d3516a4f29" />


🔁 **Program vs. process — core distinction and example**  
  – **Program**: a runnable application (example: **Chrome**).  
  – **Process**: an instance of a program that is executing (example: each open Chrome window/tab can be a separate **process**).  
  – Implication: **many processes** can originate from the same program and consume separate resources.

🧠 **Kernel responsibilities in process management**  
  – **Create** processes when programs are run.  
  – **Allocate hardware resources** such as **RAM** and CPU time to processes.  
  – **Schedule** CPU execution among processes.  
  – **Manage termination** and ensure resources are reclaimed and made available to others.

🧾 **Finite resources and the need for efficient management**  
  – Computers have limited **RAM** and **CPU** capacity; multiple programs compete for these resources.  
  – The kernel must balance allocations so the desired mix of programs can run without monopolizing hardware.

🕒 **CPU scheduling and the concept of a time slice**  
  – A **time slice** is a very short interval (typically **milliseconds**) allocated to a process for CPU execution.  
  – The CPU runs one process during its time slice, then switches to another; rapid switching creates the appearance of simultaneous execution.  
  – Clarification: scheduling is done per CPU core; on single-core systems only one process executes at a time, while multi-core systems can run multiple processes truly in parallel across cores.

🐢 **Why systems become slow — common causes and implications**  
  – One process may **consume more time slices than it should**, blocking others and reducing responsiveness.  
  – Alternatively, **too many processes** may request CPU time, exceeding what the CPU cores can handle.  
  – Implication: even with kernel scheduling, users may need to intervene (e.g., close or kill processes) to restore performance.

♻️ **Process termination and resource reclamation**  
  – When a process ends, the kernel **collects previously used resources** (RAM, file descriptors, etc.).  
  – Proper termination and reclamation are necessary so freed resources can be **reallocated** to other processes.

🧩 **System-run processes and continuous kernel oversight**  
  – The system continually runs many background processes needed for functionality; these also require scheduling and resources.  
  – The kernel must track and manage user and system processes together to maintain overall system operation.
