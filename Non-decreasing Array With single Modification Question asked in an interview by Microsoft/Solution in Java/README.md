# arsheed
import java.util.Scanner;

public class NonDecreasingOrder {
   public static void main(String[] args) {
	Scanner sc=new Scanner(System.in);
	int n=sc.nextInt();
	int a[]=new int[n];int u=0;
	a[0]=sc.nextInt();
	for(int i=1;i<n;i++) {
		a[i]=sc.nextInt();
		if(a[i-1]>a[i]) {
			u++;
		}
	}
	if(u<=1) {
		System.out.println(true);
	}else {
		System.out.println(false);
	}
	
}
}
