# Day15-with-java

Today I learned how to find a maximum number in the given array. Lets go deeper into the program......

import java.util.Scanner;
public class Day15 {
    static int max(int[] ar)
    {
        int max = 0; 
        for (int i = 0; i < ar.length; i++)
        {
            if(ar[i] > max) //comparing array element with max value
            {
                max = ar[i]; // storing array value into max
            }
        }
        return max;
}
public static void main(String[] args) {
    Scanner scan = new Scanner(System.in);
    int n = scan.nextInt();
    int[] ar = new int[n];
    for (int i = 0; i < ar.length; i++)
    {
        ar[i] = scan.nextInt();
    }
    int result = max(ar);
    System.out.println(result);  
   }
}

output:
array size: 6
array elements: 2 5 7 8 3 6
max value: 8


