# Merging-Intervals

Java 

94.07% time 
51.45% space  
O(2n)

Complexity Analysis

Time complexity : O(n^2)O(n2)

Building the graph costs O(V + E) = O(V) + O(E) = O(n) + O(n^2) = O(n^2) time, as in the worst case all intervals are mutually overlapping. Traversing the graph has the same cost (although it might appear higher at first) because our visited set guarantees that each node will be visited exactly once. Finally, because each node is part of exactly one component, the merge step costs O(V) = O(n)O(V)=O(n) time. This all adds up as follows:

O(n^2) + O(n^2) + O(n) = O(n^2)

Space complexity : O(n^2)

As previously mentioned, in the worst case, all intervals are mutually overlapping, so there will be an edge for every pair of intervals. Therefore, the memory footprint is quadratic in the input size.
