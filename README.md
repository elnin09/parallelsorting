


### Histogram Sorting in a distributed environment.

###### This project aims at sorting a large set of numbers parallely in a distributed environment. MPI is being used for communication between processes and OpenMP is being used for synchronisation among threads.


The algorithm is divided into three parts (implementation in https://github.com/elnin09/parallelsorting/blob/master/src/solution.cpp )

1) Rebalance the data on each node so that each node have equal data.
2) Find Splitters that will divide data(global data) into equal parts.
3) Move the data from nodes to the acutal node as per the splitters and then sort the data on nodes locally.
