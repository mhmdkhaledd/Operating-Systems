# Operating-Systems
## Operating Systems Summary 

![operating-system](https://github.com/user-attachments/assets/10a84a9c-d0ee-487f-8e63-8814811e5db5)
### Operating systems are an essential part of any computer systemit is the core software that manages a computer's hardware and software resources.It acts as an intermediary between the user and the computer, providing a user-friendly interfaceand handling the complex tasks of resource allocation and management.
___

### Introduction to OS  

• The computer system comprises several components: at the base level is hardware including the CPU,  
memory (RAM and ROM), and I/O devices such as keyboards and monitors.  
• The Operating System sits above the hardware, managing resources and providing a platform for system and application software.  
System software operates directly on the hardware, while application software runs on top of the OS.  
• This structure illustrates how the OS interacts with both hardware and software to facilitate computing tasks.  

![Screenshot 2024-10-21 132500](https://github.com/user-attachments/assets/9ec4a8a8-5285-4567-ad2e-6ac1d828192d)
#### there are two kinds of software :  

1 system software : used to command or modify computer hardware, operating system is also a kind of system software  

2 application software : used to perform specific task and that can be directly used by users    

• Examples of application software include word processors like Microsoft Office Word, spreadsheets like Microsoft Excel, compilers for code writing, text editors like Notepad, and web browsers like Google Chrome.

• if there is no operatig system you have to manually tell the computer hardware everything that you have do like opening applications,  
typing, displaying text, and saving files, which involves complex coding for this actions   

• so The Operating System simplifies user interaction with computer hardware by handling all this tasks. This allows users to focus on their tasks without needing to manually code every interaction with the hardware. Essentially, the OS acts as an intermediary, making computing easier and more accessible by managing complex hardware interactions.  
___
 
#### The main functions of an OS include :  
- acting as an interface between users and hardware.    
- allocating resources like the CPU, memory, hardware and I/O devices ... so when different users wants to use different resources how these resources are aloocated in such a way that every body get its share ? all this is done by operating system.  
- management of memory, security etc... this is like when we were typing in software program like word processor we have to first load it into the main memory 'RAM' and then after typing it has to be saved into the secondary memory or the hard disk.

#### types of OS include :
- batch, time-sharing, distributed, network, real-time, and multi-tasking systems, each designed for specific needs.

  ![image](https://github.com/user-attachments/assets/b425ecf8-015d-4320-8f6e-918867b33d02)

___  

### Basics of OS (Computer System Operation)  
- A modern general-purpose computer system consists of one or more CPUs and a number of device controllers connected through a common bus that provides access to shared memory.

![Screenshot (61)](https://github.com/user-attachments/assets/d13f3d94-752a-47aa-bb08-f13ab3bc690a)

#### Undertanding the role of CPUs in modern computer systems  
- A modern computer system typically includes one or more central processing units (CPUs), which are crucial for performing all computational tasks.
- The CPU, often confused with the entire computer case, is actually a small chip embedded in the motherboard responsible for calculations and processing.
- The system may also contain various device controllers connected through a common bus to manage hardware components like disks, keyboards, and printers, all of which interact with the CPU to perform their functions.

#### Memory Controller and Device Coordination in Computer Systems 
- Each of these hardwares and devices is connected to a controller This controller is responsible for the way these devices work
- Device controllers, such as USB controllers for peripherals and video adapters for displays, manage specific hardware components by regulating their operation.
- These controllers, along with the CPU, are connected through a common bus to shared memory.
- we see that they are all connected to a memory controller over here....Whenever something has to be executed or loaded It has to be loaded into your main memory.
- So what we have is the memory controller which ensures that every controller and every device gets the proper access to the memory that they need so that they can perform or work.

![Screenshot (62)](https://github.com/user-attachments/assets/59b23e9e-7d38-4f27-a970-f21810a76b98)  

___  

![Screenshot (63)](https://github.com/user-attachments/assets/54a150b4-98f4-4657-8e32-29911e40fc92)  

#### The Role and Function of the Bootstrap Program in System Startup
- The bootstrap program, also known as the bootloader, is the first program executed when a computer is powered on or rebooted. Stored in ROM (Read Only Memory).  
- It initializes the system by loading the operating system from secondary memory into the main memory.
- This program is essential for starting the operating system and facilitating the interaction between the user and the computer's hardware, ensuring that the system boots up properly and is ready for use.

#### The Bootstrap Program's Role in Loading the OS Kernel  
- The bootstrap program is responsible for initiating the computer system by locating and loading the operating system's kernel into the main memory.
- The kernel, which is the core component of the operating system, must be loaded for the OS to become operational.
- This process occurs immediately when the computer is powered on, ensuring that the system is prepared for further operations and management by the operating system.

#### Understanding the Role of Interrupts in CPU Operations  
- Interrupts are signals sent by hardware or software to the CPU, requesting it to halt its current task and address a more urgent one.
- This mechanism allows the CPU to manage multiple tasks efficiently by pausing ongoing processes to handle higher-priority operations.
- Interrupts ensure that critical tasks are addressed promptly, maintaining the system's responsiveness and functionality.

#### the Role of Interrupts in CPU Operations  
- An interrupt is a signal sent to the CPU that temporarily halts the current execution of code, allowing the system to respond to an urgent event or condition. This could be triggered by hardware (like pressing a key on the keyboard) or by software (like an error in a program).
- After receiving an interrupt, the CPU stops its current tasks, runs a specific interrupt handler to address the event, and then returns to the interrupted task.
- Interrupts enable efficient multitasking and real-time system responsiveness, ensuring that critical operations are handled immediately.

#### what is system call  
- A system call is a way for programs to request services from the operating system (OS) kernel. When a program needs to perform tasks that require access to system resources (like file operations, memory management, or process control), it cannot do so directly. Instead, it makes a system call, which switches control from the user program to the OS to execute the requested function in a safe and controlled environment.

![Screenshot (64)](https://github.com/user-attachments/assets/9158b04f-9da4-4d92-8e1f-f7870aae7ffb)

___ 

### (I/O Structure  

![Screenshot (69)](https://github.com/user-attachments/assets/ae551e6f-e070-43a1-840b-aacde26c2de6)

- An I/O device is connected to the machine by I/O port. And the devices have their device controller.
- Device controller is nothing but intermediate hardware between the machine, I/O device and OS. The OS sends instructions to the CPU to manipulate I/O devices.Then CPU sends signals to these devices via device controller
- But how does OS know what device is connected and what instructions should it send to get device working?
- When a manufacturer makes a device, they will distribute its driver program along with it. This is because the OS will never have idea about the device. The only way to interact with the device is by talking to its driver program.
- the driver program sends instructions and receives data from the device and pass it to OS for use. The OS and Driver can talk to each other simply because they are both loaded on the memory.
- Above all, is why I/O device (those shinny RGB keyboards) stops working as soon as driver program crashes

![Screenshot (67)](https://github.com/user-attachments/assets/062beda1-c676-4e06-a3a9-d3e5dffe6c02) 

#### Working of an I/O operation:
- Loading Registers: The device driver tells the device controller what to do by loading values into its registers. 
- Controller Action: The device controller reads these values from its registers and knows what operation to perform. 
- Loading Registers: The device driver tells the device controller what to do by loading values into its registers. 
- Interrupt: When done, the device controller sends an interrupt to the CPU to let it know that the operation is complete. 
- CPU Response: The CPU stops its current task, handles the interrupt, and processes the data transferred by the device controller. 
___ 

### Computer System Architecture 

- Computer systems can be categorized based on the number of general-purpose processors they utilize.
- The main types include single processor systems, which rely on one CPU to execute tasks, and multiprocessor systems, which incorporate two or more CPUs to enhance performance. Additionally, clustered systems link multiple systems to work collaboratively on tasks, thus improving efficiency and processing power.
- Each architecture has its own advantages and specific use cases, highlighting the diverse capabilities of computer systems.

#### Single Processor Systems

![Screenshot (76)](https://github.com/user-attachments/assets/11569c1c-d0e8-4e14-8538-355bdbf42eb2) 

- In a single-processor system, there is only one central processing unit (CPU) that handles all tasks and processes.
- The CPU switches between processes through a method called time-sharing or multitasking, which creates the illusion that multiple programs are running simultaneously. However, at any given moment, only one process is actively executing.
- The operating system is responsible for managing this process switching, ensuring that each task gets fair CPU time, handling priorities, and managing system resources efficiently. This type of system is simpler and more common in personal computers, but it can become less efficient under heavy workloads compared to multiprocessor systems.

![Screenshot (77)](https://github.com/user-attachments/assets/7dbaff8d-0c64-445c-b5ec-d00afe162b66)  

#### Multiprocessor systems 

- Multiprocessor systems (also known as parallel processing systems) involve multiple CPUs working together within a single computer. These CPUs share the same memory and peripherals, which allows them to handle multiple processes simultaneously, significantly increasing system performance and reliability.

#### Key features of multiprocessor systems:
- Increased Throughput: Multiple processors allow for concurrent execution of processes, improving the system’s ability to complete tasks faster.
- Fault Tolerance: If one processor fails, the system can continue working using the remaining CPUs, improving reliability.
- Shared Resources: CPUs share the main memory and I/O devices, coordinated by the operating system to prevent conflicts and ensure efficiency.
- Symmetric and Asymmetric Models:
  - Symmetric Multiprocessing (SMP): All processors are equal, sharing tasks equally.
  - Asymmetric Multiprocessing (AMP): One CPU is the master, assigning tasks to other subordinate CPUs.

   ![Screenshot (78)](https://github.com/user-attachments/assets/84ac996d-b0f4-4728-8f5e-5a09891659b4)

#### Clustered Systems

![Screenshot (79)](https://github.com/user-attachments/assets/7914f529-37af-4ba1-b96e-1fdc7a604b93) 

##### Clustered systems involve multiple independent computers (nodes) working together as a single unit. They improve performance, availability, and scalability by distributing tasks across nodes. If one node fails, others can take over, ensuring reliability (high availability). Clustered systems balance the load among nodes to handle heavy workloads efficiently. They are scalable, allowing more nodes to be added as needed. Types include high-performance clusters for intensive computations, load-balancing clusters for workload distribution, and high-availability clusters for redundancy. These systems are used in areas like cloud computing, databases, and scientific research. 

##### Clustered systems can be structured in two main ways:
- Asymmetric clustered systems, one machine operates in a hot-standby mode, monitoring the others that are actively running applications. If any of these active systems fail, the standby machine takes over, ensuring continuity.
- Symmetric clustered systems involve multiple hosts that not only run applications but also monitor each other, allowing for better resource sharing and efficiency. Symmetric configurations are generally preferred due to their collaborative nature, which optimizes resource usage and enhances system reliability.

___

### Operating System Structure 

#### Multiprogramming & Multitasking 

1. Multiprogramming:
![Screenshot (81)](https://github.com/user-attachments/assets/14fc6c41-c0ed-48a5-b88a-160a7164647c)
- Objective: To maximize CPU utilization by running multiple programs simultaneously.
- How it works: The operating system loads multiple programs into memory and switches between them. While one program is waiting for I/O (like reading from a disk), the CPU is assigned to another program.
- Benefit: It increases system efficiency by keeping the CPU busy at all times, minimizing idle time.
- Example: In a multiprogramming system, one process might be writing to a disk while another is performing calculations.

2. Multitasking:
 ![Screenshot (84)](https://github.com/user-attachments/assets/ee4c0ed6-d236-47eb-b424-f6fffa196c2f)
- Objective: To allow multiple users to interact with a computer simultaneously.
- How it works: The CPU allocates time slices to each user or task, switching between them rapidly, so each user feels as though they have the computer to themselves.
- Benefit: Provides an interactive experience for users while still efficiently managing resources across multiple programs.
- A time-sharing system allows multiple users to edit files or run programs simultaneously, each experiencing a fast response time.
![Screenshot (85)](https://github.com/user-attachments/assets/5709ccc6-10e3-4d7b-838b-05f822a7f7d6)

___

### Operating System Services

- An OS provides an environment for the execution of programs.
- It provides certain services to programs and to users of those programs. image

1. User Interface: Facilitates interaction between the user and the operating system, typically through graphical user interfaces (GUIs) or command-line interfaces (CLIs). 

2. Program Execution: Manages the execution of programs by loading them into memory, running, and terminating them. 

3. I/O Operations: Handles input and output operations, enabling interaction between the system and external devices like keyboards, printers, and storage drives. 

4. File System Manipulation: Manages file operations such as creating, deleting, reading, and writing files on storage devices. 

5. Communications: Facilitates data exchange between processes running on the same or different systems, using shared memory or message-passing mechanisms. 

6. Error Detection: Continuously monitors the system for potential errors, including hardware failures and software issues, and responds appropriately. 

7. Resource Allocation: Allocates and manages resources like CPU time, memory, and I/O devices among multiple processes. 

8. Accounting: Tracks system usage by users and applications, helping in auditing and optimizing resource usage. 

9. Protection and Security: Ensures controlled access to system resources, protecting data and system integrity from unauthorized access or breaches.


___

### User Operating System Interface 

##### the User Operating System Interface allows users to interact with the operating system to manage hardware and software resources. There are two main types of interfaces ,The CLI allows users to input commands directly, requiring them to remember specific syntax for tasks, while the GUI provides a more visual and intuitive way to interact with the system through graphical elements. Each approach has its own advantages and use cases, influencing user experience and efficiency. 

##### The GUI is characterized by its user-friendly design, allowing interaction through visual elements like desktops and menus, which enhances usability for everyday tasks. In contrast, the CLI requires users to input text-based commands, necessitating knowledge of specific command syntax. Additionally, the command interpreter's implementation varies, as some operating systems integrate it into the kernel, while others treat it as a standalone program, affecting performance and functionality. 

___ 
















  


















