# cross-compiler-collection
A collection of freestanding GNU toolchains for OS development on linux.
# Instruction
To use the compilers, you need to execute the config script, with giving as commandline arguments the command you want to execute with the compilers. That can be a compile script in the same directory, that changes the working directory and executes a make command or similar. For exsample:

A compile script

#!/bin/bash
#File compile

cd /home/user/project
make $1

Now executing the command:

$ ./config ./compile all

In this exsample, the file will execute the script to enable the compilers, and then call the compile script to compile a project via make.
