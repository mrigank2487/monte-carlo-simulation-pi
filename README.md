# Monte Carlo Simulation for Pi
#### Contains the following: ####
  ### 1. A serial approach to the estimation of Pi using the Monte Carlo Method (C++)
  ![demo](Pi/Graphs/Sequential%20-%20Iterations%20VS%20Pi.png)
  ![demo](Pi/Graphs/Sequential%20-%20Iterations%20VS%20Time.png)
  
  ### 2. A Multithreaded estimation of Pi based on the Monte Carlo Method (C++)
  
  ### 3. Using matplotlib, plots the estimated value of Pi using Monte Carlo Method (Python)
    #### 10000 Iterations
    ![demo](Pi/Graphs/10000.png)
  
  #### 100000 Iterations
  ![demo](Pi/Graphs/100000.png)
  ![demo](Pi/Graphs/100000-2.png)
  
  ### 4. A parallel computing version that estimates Pi using the Monte Carlo Method in OpenMP (C)
  ![demo](Pi/Graphs/Parallel%20-%20Threads%20VS%20Time.png)
  ![demo](Pi/Graphs/Parallel%20-%20Threads%20VS%20Pi.png)
  
  ### 5. A parallel computing version that estimates Pi using the Monte Carlo Method in MPI: Reduction & Send/Receive (C)
  
### To use OpenMP

> /usr/local/opt/llvm/bin/clang -fopenmp -L/usr/local/opt/llvm/lib main.c -o a

> ./a


### To use MPI

The best performance is achieved when the number of nodes is equal to number of cores. E.g.:

> $HOME/opt/usr/local/bin/mpicc -o pi ./mpi_pi.c

> $HOME/opt/usr/local/bin/mpirun -np 4 ./pi


You can change the number '4' to equal the number of cores you have.
You can also change the file name to whichever MPI method you want to run.

