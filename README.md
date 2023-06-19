# EK2_Pfingstprojekt_2023
Fast Point Multiplication: Non-Adjacent Form (NAF) (50 points)

Implement the normal Double-and-Add algorithm in the function double_and_add.
Implement the calculation of the NAF in the function calc_naf_representation.
Implement an adapted Double-and-Add algorithm that performs point multiplication based on the NAF. Use the function calc_naf_representation. Calculate P = k · Q for the given values using the elliptic curve P-256.
Insert count variables to output how many operations (Double, Add, Sub) are needed to calculate P = k · Q for both the Double-and-Add algorithm and the adapted Double-and-Add algorithm with NAF. State which of the two algorithms is more advantageous and explain why in a maximum of 3 sentences.
Diffie-Hellman Key Exchange with Elliptic Curves (ECDH) (50 points)

Calculate the common ECDH key KAB using the function from task 1.d for the given private ECDH parameters.
Test the speed of your implementation. Measure the total time needed to perform the calculations from task 2.a 1,000 times. Carry out this measurement for the two implemented methods for point multiplication from tasks 1.b and 1.d using the functions double_and_add and naf_double_and_add. State the two measured speeds and explain your result.
Adjust the time measurement from task 2.b so that you now measure the duration of individual calls to the functions double_and_add and naf_double_and_add. Call the functions 5,000 times each to record 5,000 individual time measurements for each of the algorithms. Use the provided function plot_performance to visualize the measured times as histograms. The generated graphic will be saved as a PNG file. Include this in your PDF submission. Discuss or briefly answer the following points:
Describe the graphic and name the main findings.
Why is it useful to repeat the speed measurements very often?
Are the observed speed differences generalizable (e.g., to other computers or for other input values)?
Implement the function ξ to generate the key KAES 128 from TAB. Decrypt the file ciphertext.hex in the project folder using the key KAES 128 = ξ(TAB) via AES128-ECB. Indicate in your solution what type of file this is.
