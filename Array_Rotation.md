```java
import java.util.Arrays;
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        //1
        Scanner scanner = new Scanner(System.in);


        //2
        System.out.println("Enter the count of the array : ");
        int count = scanner.nextInt();

        System.out.println("Enter the number of rotation : ");
        int rotation = scanner.nextInt();

        //3
        int originalArray[] = new int[count];
        int rotatedArray[] = new int[count];

        //4
        for (int i = 0; i < count; i++) {
            System.out.println("Enter element for position " + (i + 1) + " : ");
            int no = scanner.nextInt();

            //5
            originalArray[i] = no;
            rotatedArray[(i - rotation + count) % count] = no;
        }




        //6
        System.out.println("Array : " + Arrays.toString(originalArray));
        System.out.println("Rotated array : " + Arrays.toString(rotatedArray));
    }
}
.....
```
