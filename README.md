# OS161 Linux Commands
## Set the Path
`export PATH=~/cs161/bin:$PATH`
## Project Configuration
`cd ~/cs161/src`   
`./configure`   
`cd kern/conf`   
`./config ASST1`
## Building the Kernel  
`cd ~/cs161/src/kern/compile/ASST1` 'ASST1' is the new project!  
`make depend`  
`make`  
`install`  
## Running The Kernel
Change into your root directory   
`cd ~/cs161/root`  
Run the machine simulator on your operating system  
`./sys161 -w kernel`  
Shut the program down   
`p /sbin/poweroff <return>.`
## Using GDB
Run the kernel with the -w flag, then in a separate debug window  
`cd ~/cs161/root`  
`cs161-gdb kernel`  
`(gdb) target remote unix:.sockets/gdb`
### Some GDB Commands
`b line-number` adds a breakpoint  
`l line-number` lists the file  
`s` step  
`n` next line  
`r` run program  
`print var-name` prints the value of the variable  
`clear` remove breakpoints  
`set var-name = some-value` change variable value  
`watch` watch the line   
