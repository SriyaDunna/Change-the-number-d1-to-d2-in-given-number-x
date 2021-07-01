# Change-the-number-d1-to-d2-in-given-number-x

import java.util.*;  
class Swap_With {  
    public static void main(String[] args) {  
       int x, d1, d2 ;
       Scanner sc = new Scanner(System.in);  
       System.out.println("Enter the value of x");  
       x = sc.nextInt();
       System.out.println("Enter the value of d1 and d2");  
       d1 = sc.nextInt();  
       d2 = sc.nextInt();  
     int res=0, mult=1;
      while (x / 10 > 0)
        {
            int remainder = x % 10;
            if (remainder == d1)
                res = res + d2 * mult;
 
            else
                res= res + remainder * mult;
            mult *= 10;
            x = x / 10;
        }
        if (x == d1)
            res = res + d2 * mult;
 
        else 
            res = res + x * mult; 
         System.out.println("After swapping: "+res);  
       System.out.println( );  
    }    
}
