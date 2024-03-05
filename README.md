# Day15-with-java

Today I learned how to find a maximum number, to print the index of largest element in the given array. Lets go deeper into the programs......

Program to find maximum element in an array....

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

Program to print the index of largest element in an array....

 import java.util.Scanner;
public class Day15 {
    static int maxIndex(int[] ar)
    {
        int index = 0;
        int max = 0;
        for (int i = 0; i < ar.length; i++)
        {
            if(ar[i] > max)
            {
                max = ar[i];
                index = i;
            }
        }
        return index;
}
public static void main(String[] args) {
    Scanner scan = new Scanner(System.in);
    int n = scan.nextInt();
    int[] ar = new int[n];
    for (int i = 0; i < ar.length; i++)
    {
        ar[i] = scan.nextInt();
    }
    int result = maxIndex(ar);
    System.out.println(result);   
   }
}

output:

array size: 5
array elements: 1 4 8 2 5
index of max value: 2

