## Sequences

You are on a company visit to Shopee. During the office tour, you noticed that there seems to be a random scribbling on one of the walls. After looking at it closely, you noticed it is actually an algorithm question! Below is the question:

> You are given N functions f(i, j) with parameters Ai, Bi, Ci, where the value of f(i, j) is equal to Ai x j2 + Bi for each 1 ≤ j ≤ Ci. Find how many sequences (i1, j1), (i2, j2), … , (iM, jM) of length M are there in which the following holds:
f(i1, j1) + f(i2, j2) + … + f(iM, jM) is divisible by K
Two sequences are different if there is at least one index k, such that ik ≠ ik’ or jk ≠ jk’

You quickly take note of the question, as maybe it is a draft for an interview question. Solve the question to increase your chance of acing the future interview at Shopee!

## Input

The first line contains 3 integers N (1 ≤ N ≤ 5,000), M (1 ≤ M ≤ 1,000,000,000), and K (1 ≤ K ≤ 2,000).

The next N lines each contains 3 integers Ai, Bi, (0 ≤ Ai, Bi < K) and Ci (1 ≤ Ci ≤ 1,000,000,000), denoting the parameters for the i-th function.

## Output

One line containing a single integer, the number of the sequence. Since this number can be very large, output its value modulo 109+7.

SAMPLE INPUT
3 2 6
0 3 2
1 2 3
2 5 1

SAMPLE OUTPUT
12

##### Explanation
Below are all the possible sequences:

(1, 1), (1, 1)
(1, 1), (1, 2)
(1, 1), (2, 1)
(1, 2), (1, 1)
(1, 2), (1, 2)
(1, 2), (2, 1)
(2, 1), (1, 1)
(2, 1), (1, 2)
(2, 1), (2, 1)
(2, 2), (2, 2)
(2, 3), (3, 1)
(3, 1), (2, 3)