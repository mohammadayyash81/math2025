Extracting Prime Numbers from a Given Number in R
This R script is designed to extract prime digits from a given number. It consists of two main functions: one for checking whether a number is prime and another for extracting prime digits from the entered number.

1. Checking if a Number is Prime
The function is_prime(n) determines whether a given number n is prime. It follows these steps:

If n is less than 2, it returns FALSE since numbers less than 2 are not prime.
If n is exactly 2, it returns TRUE, as 2 is the smallest prime number.
If n is an even number greater than 2, it returns FALSE because all even numbers (except 2) are composite.
Otherwise, it checks divisibility by iterating from 3 up to the square root of n. If n is divisible by any of these numbers, it is not prime.
2. Extracting Prime Digits
The function extract_primes(num) extracts prime digits from a given number num using the following steps:

Converts the number into a string and then splits it into individual digits.
Converts these digits back into numeric values.
Filters out the prime digits using the is_prime() function.
Returns the extracted prime digits as a vector.
3. Example Usage
When calling the function with an example number such as 237465, the program:

Split the number into individual digits: [2, 3, 7, 4, 6, 5]
Identifies which of these digits are prime: [2, 3, 7, 5]
Returns [2, 3, 7, 5] as output.
