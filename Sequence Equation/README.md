# Sequence Equation
Given a sequence of n integers, p(1),p(2),....,p(n) where each element is distinct and satisfies 1 <= p(x) <= n. For each x where 1 <= x <= n, find any integer y such that p(p(y))=x and print the value ofy  on a new line.<br>
For example, assume the sequence p = [5,2,1,3,4]. Each value of x between 1 and 5, the length of the sequence, is analyzed as follows:<br>

1. x = 1 = p[3],p[4]=3, so p[p[4]] = 1<br>
2. x = 2 = p[2],p[2]=2, so p[p[2]] = 2<br> 
3. x = 3 = p[4],p[5]=4, so p[p[5]] = 3<br>
4. x = 4 = p[5],p[1]=5, so p[p[1]] = 4<br>
5. x = 5 = p[1],p[3]=1, so p[p[3]] = 5<br>
<br>
The values for y are [4,2,5,1,3].

## Function Description

Complete the permutationEquation function in the editor below. It should return an array of integers that represent the values of y.<br>
permutationEquation has the following parameter(s):<br>
p: an array of integers<br>

## Input Format

The first line contains an integer n, the number of elements in the sequence.<br>
The second line contains n space-separated integers p[i] where 1 <= i <= n.

## Constraints
1 <= n <= 50<br>
1 <= p[i] <= 50, where 1 <= i <= n.<br>
Each element in the sequence is distinct.

## Output Format

For each x from 1 to n, print an integer denoting any valid y satisfying the equation p(p(y))=x on a new line.

### Sample Input 0
3<br>
2 3 1<br>

### Sample Output 0
2<br>
3<br>
1
