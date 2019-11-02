# arsheed
import java.util.Scanner;
import java.util.TreeMap;

public class StackProble {
   public static void main(String[] args) {
	Scanner sc=new Scanner(System.in);
	int n=sc.nextInt();
	int a[]=new int [n];
	
	for(int i=0;i<n;i++) {
		a[i]=sc.nextInt();
		int max=Integer.MIN_VALUE;
		for(int j=i-1;j>=0;j--) {
			if(a[j]>max && a[j]<a[i]) {
				max=a[j];break;
			}
		}
		if(max==Integer.MIN_VALUE) {
			System.out.print(-1+" ");
		}else {
			System.out.print(max+" ");
		}
	}
	
	
}
}
