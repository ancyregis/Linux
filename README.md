# Linux

23/2/24

GNU - gnu's not linux
OSS - source  code is free, can modify

Red hat - networking, Administration purpose
stream os
fedora - education purpose

Linux  is monolethic kernal , not an os

 ancy @ ancy: ~ $ username hostname path

two types of path

relative path --> :$CD../D1/D2/D3 ---> :$CD . /D1/D2/D3
absolute path ---> from root to folde is called absolute path
COMMANDS sudo apt -get install tree tree>treee-file vim tree-file rm tree-file rm-rf --->recursive forceful ls -l ls -la ----->hidden files which ls which cd CD -----> it is internal command ls -----> it is external command No manual page for internal commands

man ls ---> man command is used to read the ls command details man man man hier type cd type ls help cd

sudo su p(w) exit ls cd rtc tree tree>tree-file vim tree-files --->convert all to files


COMMANDS
sudo apt -get install tree
tree>treee-file
vim tree-file
rm tree-file
rm-rf  --->recursive forceful
ls -l 
ls -la ----->hidden files
which ls
which cd
CD -----> it is internal command
ls  -----> it is external command
 No manual page for internal commands

 man ls ---> man command is used to read the ls command details
 man man
 man hier
 type cd 
 type ls 
 help cd

 sudo su
 p(w)
 exit 
 ls
 cd rtc
 tree
 tree>tree-file
 vim tree-files  --->convert all to files


 DESCRIPTORS
 Using file descriptors only we can access the file.
 0 -standard input, keyword
 1 -standard  output 
 2 -standard error
three descriptors already open for a file
open system calls return  value will be FILE DESCRIPTORS

for both we are using open sys call (already exists OPEN)(new create OPEN)





SDCARD BOOT

 sudo minicom
 password -> click the button
 printenv
 editenv bootargs
 edit:console=ttyso,115200 console=ttyo earlyprintk root=/dev/MMCBKLP2 rw rootwait
 saveenv
 boot 
 root


 TFTP PROTOCOL

 touch /var/lib/tftpboot/ filename
 ls /var/lib/tftpboot
 echo "Rathinam" >/var/lib/tftpboot/filename

 BOOT TERMINAL

 sudo minicom
  check wired connection
  root
  ifconfig eth0 192.168.1.34
  tftp -r filename -g 192.168.1.30
  chmod 777 filename
  ls
  cat filename

  16/4/2024

  THREADS
  A thread refers to a basic unit of execution within a PROCESS. Threads share the same memory space and resources of the process they belog to, allowing them to communicate easily with each other.
  A traditional/heavyweight process has a SINGLE thread of control.
  If a  process has MULTIPLE threads of control, it can perform morebthan one task at a time.Here the each thread has their own separate registers and stack.
  Thread comprises of ThredID

  BENEFITS
  =>Responsiveness
  =>Resourse sharing
  =>Economy
  =>Utilization of multiprocessor architecture

  17/4/2024

  Resource sharea according to time is CONCURRENCY
  parallelism = time decrease
  singalarism = time decrease
  concurrency = time increase
  To implement condition variables we have MUTEX

  THREAD SYNCHRONIZATION
   Hardest and most important aspect of multithreading is thread synchronization.
   (Critical synchronization) operations like [read-write or write -write]
   To overcome critical synchronization MUTEX
                 mutex = only one thread can work at a time.
   threadku mutual exclusion kudukarathuku mutexes

   how mutex works = if t1 is inside it will lock it will unlock after completing the work.

   example:
           pthread_mutex_t mutex;
           foo(){
           pthread_mutex_lock[&mutex];  //lock
           /*critical section*/
           pthread_mutex_unlock[&mutex] //key unlock

18/5/2024
  
