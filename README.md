# About 
"PCRTT" is a posix compliant port of the CSA-Rainbow-Table-Tool from colibri.

# Work in progress.
There is nothing working out of the box.
You can generate rainbow table, but it is not certified that all is 
working correctly for now (I have not tested the resulting table from OpenCL/CPU)

# Why the port ? :
1) Firstly, because I wanted to try to port it.
2) It was a good way of training, to learn Cuda, OpenCL, and many other
   SDK/Tool chain, Algorithm, etc.

# Features (work in progress)
GUI support :
- FLTK (using fluid)
- GTK (using glade)
- Console (ncurses)

Algorithm (GPU/CPU) :
- Cuda (Original code from colibri)
- ported to OpenCL
- VULKAN (when possible)
- A thread pool and a CPU only was added (3 kCW/sec on a Corei7 with 8 thread)
* Parallel sort :
 -  the one from https://github.com/sol-prog
 -  lib Intel TBB
 - STXXL

# libdvbcsa (v1.1.0)
 Patched (thank to the author, from the vlc forum)
 to support SSE3, and NEON opcode.

# The goal
To make the most perfect posix compliant tool as possible.
To use the fastest algorithm possible. (using sse, avx, gpu, whatever...)
To use external sort algorithm (using stxxl nor libextsort).

# Original Author
Copyright (C) 2012  Colibri <colibri.dvb@googlemail.com>  
http://colibri.net63.net/ alias http://colibri-dvb.info/

# Logo Copyright
(C) 2012 Colibri <colibri.dvb@googlemail.com> 
(Modified "a bit" with gimp)

# Disclaimer
I do not condone or endorse piracy in any form.
This port are simply for informational\educational purposes only.
I am not responsible for what you do with the tool/sotware presented herein.
