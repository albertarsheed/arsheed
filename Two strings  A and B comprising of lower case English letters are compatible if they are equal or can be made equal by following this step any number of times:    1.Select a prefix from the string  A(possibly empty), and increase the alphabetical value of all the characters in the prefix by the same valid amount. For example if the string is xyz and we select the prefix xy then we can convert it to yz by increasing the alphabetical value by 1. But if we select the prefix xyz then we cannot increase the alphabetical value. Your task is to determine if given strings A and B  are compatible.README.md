# arsheed
import java.util.Scanner;

public class DooStringsKaPanga {
   public static void main(String[] args) {
	Scanner sc=new Scanner(System.in);
	String s1=sc.next();
	String s2=sc.next();
	int z=0;
	int a[]=new int[s1.length()];
	if(s1.length()!=s2.length()){
	    System.out.println("NO");
	}else{
	for(int i=0;i<s1.length();i++) {
		a[i]=s2.charAt(i)-s1.charAt(i);
	
	}
	for(int i=0;i<s1.length()-1;i++) {
		if(a[i]>=a[i+1]) {
			
		}else {
			z++;
		}
	}

	if(z==0) {
		System.out.println("YES");
	}else {
		System.out.println("NO");
	}
}}
}
