# arsheed
import java.util.*;

public class Problem1 {
    public static void main(String[] args) throws Exception {
        Scanner sc=new Scanner (System.in);
        int t=sc.nextInt();
        while(t-->0) {
        	int n=sc.nextInt();
        	TreeSet <Integer>tr=new TreeSet();
        	int me=sc.nextInt();
        	int a[]=new int[me];
        	for(int i=0;i<me;i++) {
        		a[i]=sc.nextInt();
        		tr.add(a[i]);
        	}
        	int fr=sc.nextInt();
        	int b[]=new int[fr];
        	for(int i=0;i<fr;i++) {
        		b[i]=sc.nextInt();
        		tr.add(b[i]);
        	}
        	if(n==tr.size()) {
        		System.out.println("YES");
        	}else {
        		System.out.println("NO");
        	}
        }
    }
}
