## The core components of Linux (kernel, user space, init/systemd)

Linux operating system is divided into 2 core spaces, Kernel space and user space. 
  - ### Kernel
    It is the brain of OS which sits in the hardware and manages resources like CPU, Memory and Disk usage. Its a gate keeper for every hardware call.
  - ### UserSpace
    Its where your application resides and communicates with kernel via system calls.
  - ### Init/systemd
    The very first process started by kernel (PID 1) its the parent of all other process in the system  

## How processes are created and managed
  - In Linux processes are managed through parent-child relationship by using fork() and exec().
    fork() - this system call creates First the process is forked from parent process creating an exact duplicate which is a child process and then child process calls exec() call

## What systemd does and why it matters
  - It is the first process that starts and last to end 

  - It initialises the system and start backgorund service like daemons required to run OS

  - it monitors your services and if database or app services crash, systemd can easily restart.

  - It starts services in parallel, instead of one by one . making the boot process much faster
