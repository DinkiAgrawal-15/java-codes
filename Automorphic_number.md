```java
import java.util.*;
public class Main{
    public static void main(String a[]){
        int num;
        int n;
        int r;
        int t;
        int sq;
        boolean equal=false;
        Scanner sc=new Scanner(System.in);
        n=sc.nextInt();
        num=n;
          sq=n*n;
          t=10;
          System.out.println("\n square of "+n+" is" +sq);
        while(n>0){
            r=sq%t;
            if(num==r){
                equal=true;
                break;
            }
            n=n/10;
            t=t*10;
        }
        
        if(equal==true){
                    System.out.println(num+" Number is Automorphic");
        }else{
                                System.out.println(num+" Number is not  automorphic");

        }
    }
}
```
