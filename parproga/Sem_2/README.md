# Compile

OpenMP:

    clang -Xclang -fopenmp -L/opt/homebrew/opt/libomp/lib -I/opt/homebrew/opt/libomp/include -lomp hello.c -o hello
    ./hello <agrs>

MPI:

    mpicc -lm hello.c -o hello
    mpirun -np <threads> ./hello <args>

Single thread compile:

    gcc main.c -o main
    ./main <args>

Diff:

    diff result_openmp.txt result_single.txt
