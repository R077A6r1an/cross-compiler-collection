# cross-compiler-collection
A collection of freestanding GNU toolchains for OS development on linux.
# Instruction
Execute the config script, to enable the toolchain in your current terminal session. After this, you can use the compilers needed for your platform in the current terminal session, with commands like:

$ arm64-gcc -c main.c

Means, the target arch, and then seperated throught a '-' character the compiler programm you wan't to use.
The compilers are availeable for x86_64 and aarch64 ( arm64 ) host environments on linux, and for target just the listed target architectures listet by executing the script.

Note that everytime you wan't open a new shell session, you need to execute the config script, to enable the toolchain. Alternative, you can set the environment variable in the bash config file (normaly /etc/environment) with the value of the following commands:

$ ./config
$ echo $PATH

The output of the last command must be replaced with the value setted in the config file.
# Troubleshooting
If any error occures, write an issue over it, and I'll just fix it.
