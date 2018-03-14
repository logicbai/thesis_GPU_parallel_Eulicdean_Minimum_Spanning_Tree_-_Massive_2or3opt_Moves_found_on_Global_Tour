# thesis_GPU_parallel_Eulicdean_Minimum_Spanning_Tree_-_Massive_2or3opt_Moves_found_on_Global_Tour
In this thesis, we propose two new branches of research interests to graph minimization problems, first one, parallel Euclidean minimum spanning tree/forest (EMST/EMSF) algorithms for input graph that only possesses vertexes as input; second one, multiple 2-opt / 3-opt moves that are found on the same global tour or in the same integral Euclidean space for traveling salesman problems (TSP). To respond these two research interests, firstly, we propose a newly proposed hierarchical EMST/EMSF algorithm that combines the cellular partition based nearest neighbor search with Borůvka's algorithm, which provides an alternative hierarchical data clustering solution to various optimization problems whose input graph only contains vertexes with uniform or bounded data distribution. Secondly, a judicious decision making methodology of offloading which part of the k-opt heuristic works in parallel on Graphics Processing Unit (GPU) while which part remains sequential, called parallel local search but sequential selection, in order to simultaneously execute, without interference, massive 2-/3-opt moves that are globally found on the same TSP tour or the same Euclidean space for many edges as well as keeping high performance on GPU side. This methodology for multiple 2-/3-opt moves is judicious since intervention of a sequential O(N) time complexity tour reversal operation is unavoidable when using arrays as TSP tour data structure for high performance GPU parallel k-opt implementation that considers coalesced memory access and usage of limited on-chip shared memory; it is valuable since our newly proposed non-interacted 2-/3-exchanges set partition algorithm that takes O(N) sequential time complexity, and a new TSP tour data structure, array of ordered coordinates-index, for GPU high performance local search implementation. All these proposed parallel solutions work on GPU with parallel technique of decentralized control, data/task decomposition, GPU on-chip shared or off-chip global memory.
