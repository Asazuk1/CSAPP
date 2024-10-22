##### phase_1: Border relations with Canada have never been better.
read the assembly code, the answer is in 0x402400

##### phase_2: 1 2 4 8 16 32
read_six_numbers, then a for loop
maybe: for (int i = 1; i <= 32; i *= 2)

##### phase_3: 0 207
sscanf indicates %d %d, let's assign them as x, y
x should be less than 7
the remain assembly code may be a case statement, 0 207 can pass the test

##### phase_4: 0 0
sscanf indicates %d %d, let's assign them as x, y
x must be 0
y = func4(x, 0, 14)
func4 is a binary search function, return the depth of x in a binary tree(0, 14)

##### phase_5: 9(I)/(O)>(N)5(E)6(F)7(G)
these are all correct answers: 9/>567, IONEFG, 9ON56G ...
phase_5 needs a string, and the lengh must be 6, name it as s
phase_5 implements something like a hash table
s -> s_result, s_result is in 0x40245e, "flyers"
a string in 0x4024b0 is "maduiersnfotvbyl", name it as s1
should make sure (s[i] & 0x0F) == (s_result[i]'s index in s1)
e.g: s_result[0]: f, its index in s1 is 9 because s1[9] == 'f', so you can refer that s[0] must be 9 or I

##### phase_6: 4 3 2 1 6 5
read_six_numbers, input 6 different numbers between 1 and 6
each input x will be changed to 7 - x, and just guarantee the array after this change is 4 3 2 1 5 6

##### secret_phase:
I don't want to solve it anymore! 