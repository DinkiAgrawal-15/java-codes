```java
// Java Program to Compare two Boolean
// Arrays using Naive approach

import java.io.*;

class Main{
	public static void main(String[] args)
	{
		// initializing both the boolean arrays
		boolean[] a = new boolean[] { true, true, false };
		boolean[] a1 = new boolean[] { true, true, false };

		// Displaying Array1
		System.out.println("Array1...");
		for (int i = 0; i < a.length; i++)
		{
			System.out.println(a[i]);
		}
		
		// Displaying Array2
		System.out.println("Array2...");
		for (int j = 0; j < a1.length; j++)
		{
			System.out.println(a1[j]);
		}
		
		// Comparing both the arrays
		for (int i = 0; i < a.length; i++)
		{
			// if any element is found different we will
			// print our ans and exit the program.
			if (a[i] != a1[i])
			{
				System.out.println(
					"Both the arrays equal ");
				System.exit(0);
			}
		}
		
		System.out.println("Both the arrays equal ");
	}
}
```
