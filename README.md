#  Single Processor System

The goal of this project is to create a simple system using gem5. In this system, we have only one simple CPU core. This CPU core will be connected to a memory bus and we have a memory channel, also connected to the memory bus.

## Building on Ubuntu
1. The required dependencies can be installed:

   <code>$ sudo apt-get install swig gcc m4 python python-dev libgoogle-perftools-dev mercurial scons g++ build-essential </code>
2. Clone gem5 source and build gem5 by using scons:

   <code>$ hg clone http://repo.gem5.org/gem5 </code> <br />
   
   <code>$ cd gem5/ </code> <br />
   
   <code>$ scons build/X86/gem5.opt -j + NUMBER OF CPUs ON YOUR PLATFORM ( for example -j2 ) </code> <br />
 
3. Clone the repository.
4. Run gem5 from the root gem5 directory as:
   
   <code>$ gem5/build/X86/gem5.opt system/simple_system.py --cmd=test/bin/test1 </code>


## Links
1. [gem5 Documentation](https://www.gem5.org/documentation/)
2. [gem5 Tutorial](https://course.ece.cmu.edu/~ece740/gem5/index.html)
