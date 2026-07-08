if i and j are in different components (cycles), then swapping their values or other endpoint, would result in 1 less cycle

if i and j are in same component, then swapping their values would result in 1 more cycle created

how do we calculate the number of inversions?
I mod 2 = 0 : permutation is even
I mod 2 = 1 : permutation is odd

we define the parity of permutation using no. of inversions (I)

Even Permutation: Has an even inversion count. It takes an even number of swaps to return the elements to their original order.
Odd Permutation: Has an odd inversion count. It takes an odd number of swaps to return the elements to their original order.

Mathematical definition: For a permutation \(\pi \), an inversion is a pair of indices \((i, j)\) such that \(i < j\) but \(\pi(i) > \pi(j)\).

f(a) : count of total cycles in a graph

f(a) + I = invariant

I = f(a) + n (mod 2)
since f(a) can be calculated in linear time using dfs, we can calculate the number of inversions (I) in linear time too

compose two permutations: a o b (input permutation)
a and b are some permutations which is a rearrangement operation on input permutation

flip every edge gives the inverse permutation

