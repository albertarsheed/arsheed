# arsheed

import java.util.*;

class TestClass {
    public static void main(String args[] ) throws Exception {
      
        Scanner sc= new Scanner(System.in);
        int n=sc.nextInt();
        int k=sc.nextInt();
        int a[]=new int[n];
        for(int i=0;i<n;i++){
            a[(n+i-k)%n]=sc.nextInt();
            
        }
      for(int i=0;i<n;i++){
            System.out.print(a[i]+" ");
            
        }

    }
}
