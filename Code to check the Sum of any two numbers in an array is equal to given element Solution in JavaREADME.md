# arsheed
import java.util.*;

public class SumOfPresent {
   public static void main(String[] args) {
	Scanner sc =new Scanner(System.in);
	int n=sc.nextInt();int k=sc.nextInt();
	int a[]=new int[n];
	for(int i=0;i<n;i++) {
		a[i]=sc.nextInt();
	}
	HashSet<Integer> hmap=new HashSet();int j=0;
	for(int i=0;i<n;i++) {
		int t=k-a[i];
		if(hmap.contains(t)) {j++;
			System.out.println(a[i]+" "+t);break;
		}
		hmap.add(a[i]);
	}
	
	if(j==0) {
		System.out.println("Elements not Present: ");
	}
	
	
}
}
