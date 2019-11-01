# arsheed

//import for Scanner and other utility classes
import java.util.*;

 class HeyBabes {
    public static void main(String args[] ) throws Exception {
      
        Scanner sc= new Scanner(System.in);
        int n=sc.nextInt();
        int k=sc.nextInt();
        long a[]=new long[n];long max=0;
        for(int i=0;i<n;i++) {
        	a[i]=sc.nextLong();
        	if(max<a[i] ) {
        		max=a[i];
        	}
        }
        if (k == n || (n == 1 && k % 2 == 1))
        	System.out.println(-1);
        	else if (k>n+1)
        	System.out.println(max);
        	else{
        	max=-1;
        	for (int i= 0;i<k-1;i++)
        	 {max=Math.max(max,a[i]);}
        	System.out.println(Math.max(max,a[k]));
        	
        	}
    }
}
