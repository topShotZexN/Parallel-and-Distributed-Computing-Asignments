# Parallel-and-Distributed-Computing-Asignments
Lab Assignments related to openMP and MPI.

Questions:
  Assignment1:
    Write a simple OpenMP program to demonstrate the parallel loop construct.
      a. Use OMP_SET_THREAD_NUM( ) and OMP_GET_THREAD_NUM( ) to find the number of processing unit
      b. Use function invoke to print ‘Hello World’
      c. To examine the above scenario, the functions such as omp_get_num_procs(), omp_set_num_threads(), omp_get_num_threads(),                  omp_in_parallel(), omp_get_dynamic() and omp_get_nested() are listed and the explanation is given below to explore the concept          practically.

        omp_set_num_threads() takes an integer argument and requests that the Operating System provide that number of threads in                 subsequent parallel regions.

        omp_get_num_threads() (integer function) return s the actual number of threads in the current team of threads.

        omp_get_thread_num() (integer function) returns the ID of a thread, where the ID ranges from 0 to the number of threads minus 1.         The thread with the ID of 0 is the master thread.

        omp_get_num_procs() returns the number of processors that are available when the function is called.

        omp_get_dynamic() returns a value that indicates if the number of threads available in subsequent parallel region can be                 adjusted by the run time.

        omp_get_nested() returns a value that indicates if nested parallelism is enabled.

  Assignment2:
    Write a simple OpenMP program to demonstrate the use of for, private and shared clause.
      a. Sum of ‘n’ array Using Private and Shared Clause
      b. Product of ‘n’ array using Private and Shared Clause
      
  Assignment3:
    Write a simple OpenMP program to employ a ‘reduction’ clause to express the reduction of a for loop. In order to specify the             reduction in OpenMP, we must provide
      1. An operation (+ / * / o)
      2. A reduction variable (sum / product / reduction). This variable holds the result of the computation.
      
  Assignment4:
    Write a simple OpenMP program to employ a ‘Work Sharing’ clause to assign each thread an
    independent set of iterations. In order to explore its practical use, you are advised to read and understand the following               statements.
      1. Assign each thread an independent set of iterations;
      2. Threads must wait at the end
      3. Can combine the directives:
      4. #pragma omp parallel for
      5. Only simple kinds of for loops:
        a. Only one signed integer variable
        b. Initialization: var=init
        c. Comparison: var op last op: , <=, >=
        d. Increment: var++, var--, var+=incr, var-=incr, etc.
  
  Assignment5:
    Write a simple OpenMP program to demonstrate the use of schedule clause
      a. Statically assign the loop iterations to threads
      b. Dynamically assign one iteration to each threads
      
  Assignment6:
    Write a simple OpenMP program to demonstrate Arithmetic Operation using Section Clause.
  
  Assignment7:
    Write a simple OpenMP program to demonstrate Linear Search using Section Clause.
    
  Assignment8:
    Write a basic MPI program.
  
  Assignment9:
    Write a basic MPI program to understand MPI_Send and MPI_Recv functions. Build and Execute Its Logical Scenario. Depict the             screenshots along with proper justification.
  
  Assignment10:
    Write a MPI program that takes data from process zero and sends it to all of the other processes by sending it in a ring and its         logical approach is based on MPI. That is, process i should receive the data and send it to process i+1, until the last                 process is reached. Analyse its key factors in terms of network application system. Assume that the data consists of a single           integer. Process zero reads the data from the user.
  
