Tutorial
--------
We use loops in programming to repeat execution of a block of code instead of repeating the entire code. In C ++ we have 3 types of loops, for-loops, while loops, do-while loops.

### "for" loop

if we know the exact number of times to repeat the loop for, we use a "for" loop. The syntax has 4 parts, the initialization, test expression, modifying expression and the code block to be executed in loop. 

    // syntax of for loop
    for (initialization; test condition; update) {
        // body of the loop
    }

Here's an example

    // prints Hello C++ for 10 times
    for(int i = 0; i < 10; i++)
    {
        cout << "Hello C++" << endl;
    }

In the above example, we are declaring a loop variable i, which is initialised to 0. 

Then if the test condition turns out to be true, we continue with the loop and execute the body of the loop.  After every iteration of the loop, the modifying expression is run ( Here we are using i++ which increments the value of i by 1 in every step ). We continue this process till the test condition turns out to be false i.e. when i becomes 10 in the above loop.

The loop can be read as "As long as i is less than 10, run the below Code".

We can also write the initialisation part before and modifying expression in the body of the loop

    // print numbers 0 - 9
    int i = 0;
    for( ; i < 10 ; )
    {
        cout << i << endl;
        i++;
    }

The for loop in C++ can also be used to iterate over an array just as in python as shown in the example below.

    // print the array elements 
    int arr[] = {1,2,3,4,5,6};
    int n;
    for(n : arr)
    {
        cout << n << endl;
    }

Exercise
--------
Try to print all the even numbers below 20 using a for loop.

Tutorial Code
-------------
#include <iostream>
using namespace std;

int main()
{
    # your code goes here.
    return 0;
}

Expected Output
---------------
0
2
4
6
8
10
12
14
16
18

Solution
--------
#include <iostream>
using namespace std;

int main()
{
    int i;
    for(i = 0; i < 20; i ++)
    {
        if(i % 2 == 0)
        {
            cout << i << endl;
        }
    }
    return 0;
}