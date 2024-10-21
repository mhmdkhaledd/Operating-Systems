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














