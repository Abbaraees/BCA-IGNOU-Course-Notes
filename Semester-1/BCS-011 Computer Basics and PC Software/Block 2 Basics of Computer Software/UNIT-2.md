# OPERATING SYSTEM
An operating system is system software which may be viewed as an organized collection of software consisting of procedures for operating a computer and providing an environment for execution of programs. It acts as an interface between users and the hardware of a computer system.

There are many important reasons for studying operating systems. Some of them are:
1) User interacts with computer through the operating system in order to
accomplish his/her task since it is his/her primary interface with a computer.
2) It helps users to understand the inner functions of a computer very closely.
3) Many concepts and techniques found in the operating system have general applicability in other applications.

## OBJECTIVES
After going through this unit, you should be able to:
- describe Operating Systems concepts;
- list components of an operatin system;
- Describes services provided by OS (Operating System) components;
- Describe in brief evolution of an operating system

## THE CONCEPT OF OPERATING SYSTEM
The basic objectives of an operating system are to make the computer system convenient to use and to utilize computer hardware in an efficient manner.

We can define an operating system as a large collection of software, which manages the resources of the computer system, such as memory, processor, file system and input/output devices.

So how does operating system execute a command? In order to execute a command OS does the following steps:
- It accepts a command from a user through mouse clicks or from the keyboard. Through a port number it is able to recognize what is the source of input.
- It must interpret these commands and take actions accordingly.
- It must provide a file system that can interpret the name of the program being requested and determine the location of the file on secondary storage device for example.
- It must read the appropriate blocks from the device into memory. Only then can the operating system transfer control to the program being executed.

### Facilities operating system provides to the users and programs:
- The operating system provides interfaces for the user (keyboard, mouse, clicks, and pen drive) and also for the user’s programs.
- It provides file system support to manage huge volume of data in to secondary storage device.
- It provides I/O services that can be used by every program.
- It provides boot-strapping or Initial Program Load (IPL) to start a computer
- It manages all kinds of errors and also supports error recovery mechanisms
- It provides networking services.
- It provides the environment (allocation of memory, I/O devices and CPU time) for concurrent processing. 

The operating system is commonly divided into **resident** and **non resident** parts. Some operating system services are critical to the operation of the system and must be **resident** in memory all the time. 

The critical programs are loaded into memory by the bootstrap loader at start-up time and will remain resident as long as the computer is running.

The memory resident components of an operating system are commonly known as the **kernel** of the operating system.

**Diskless workstations** are also known as **thin clients**.

## OPERATING SYSTEM SERVICES
### Command Processor and User Interface
To the user, the most important and visible services provided by the OS is the user interface and the capabilities that it provides to execute commands which may not be a part of OS.

Different types of user interface exist. The most common are the graphical user interface, or GUI, and the command line interface. The graphical user interface accepts commands primarily in the form of drop-down menus, mouse movements, and mouse clicks. The command line interface relies on typed commands which provide direct access to various methods within operating system such as File system, I/O system, and network services. UNIX allows certain class of users called superusers to use some kind of commands for changing the platform or access rights.

### File Management
The concept of a file is central to the effective use of a computer system. A file is generally loosely defined as a collection of related information such as students records employee database. It might contain graphical usage. A file may be organized internally into records or it may simply be a stream of bytes. A file constitutes a logical unit of storage, that is, logical to the person or program using the file.

The file management system provides and maintains the mapping between a file logical storage needs and the physical location where it is stored. Users and programs simply access the files by the name, and the file management system handles the details.

### Input/Output Services
Every operating system, large or small, provides input/output services for each device in the system. The operating system includes I/O device driver programs for each device installed on the system. These drivers provide services to the file management system and are also available, through the API, to other programs for their use. The I/O device drivers accept I/O requests and perform the actual data transfers between the hardware and specified areas of memory.

### Process Control Management
A process is an executing program. It is considered the standard unit of work within a computer system. Every executing program is treated as a process.

The operating system performs various functions with processes, including scheduling and memory management, by providing the various services.

Systems also provide communication capability between different processes. Processes may cooperate with each other by sending messages back and forth using interprocess messaging services.

Many modern systems further break the process down into smaller units called threads. A thread is an individually executable part of a process. It shares memory and other resources with all other threads in the same process, but can be scheduled to run separately from other threads

### Memory Management
The purpose of the memory management system is to load programs into memory in such a way as to give each program loaded the memory that it requires for execution.

## A BIT OF HISTORY
### Serial Processing
During the late 1940s to the mid-1950s, the programmer interacted directly with computer hardware; there was no operating system. These machines were run by operators from a console, consisting of displays lights, toggle switches, some form of input device and a printer. Programs in machine code were loaded via a card reader.

### Simple Batch Systems
The central idea behind the batch processing system was the use of a piece of software known as the monitor. With the use of this type of operating system, the user no longer had direct access to the machine. Rather, the user submitted the job on cards or tape to a computer operator, who batches the jobs together sequentially and places the entire batch on an input device, for use by the monitor. Many important breakthroughs in operating system design occurred in the early 1960s which laid the foundation for design of modern operating system.

### Time Sharing System
Just as multiprogramming allows the processor to handle multiple batch jobs at a time, multiprogramming can be used to handle multiple interactive jobs. In this latter case, the technique is referred to as time sharing, because the processor’s time is shared among multiple users. In time sharing system, multiple users simultaneously access the system through terminals, with the operating system interleaving the execution of each user program in a short burst or quantum of computation.