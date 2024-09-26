# Count-the-digits-
#include <stdio.h>

// Find the count of digits
int findCount(int n)
{
      // For digit 0
      if(n == 0)
          return 1;
      
    int count = 0;

    // Remove last digit from number
    // till number is 0
    while (n != 0) {

        // Increment count
        count++;
        n /= 10;
    }

    // return the count of digit
    return count;
}

// Driver program
int main()
{
    int n = 98562;
    printf("Count of digits in %d = %d\n", n, findCount(n));
    return 0;
}
