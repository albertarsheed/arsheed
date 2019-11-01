# arsheed
import java.util.Arrays;
import java.util.Scanner;

public class heyYou {
   public static void main(String[] args) {
	Scanner sc=new Scanner(System.in);
	while(sc.hasNext()) {
		String s1=sc.nextLine();
		String s2=sc.nextLine();
		char a1[]=s1.toCharArray();
		char a2[]=s2.toCharArray();
		for(int i=0;i<a1.length;i++) {
			if(Character.isUpperCase(a1[i])) {
				a1[i]=Character.toLowerCase(a1[i]);
			}
		}
		for(int i=0;i<a2.length;i++) {
			if(Character.isUpperCase(a2[i])) {
				a2[i]=Character.toLowerCase(a2[i]);
			}
		}
		Arrays.sort(a1);
		Arrays.sort(a2);
		String r1="";
		String r2="";
		for(int i=0;i<a1.length;i++) {
			if(a1[i]>='a'&&a1[i]<='z') {
				r1=r1+a1[i];
			}
		}
		for(int i=0;i<a2.length;i++) {
			if(a2[i]>='a'&&a2[i]<='z') {
				r2=r2+a2[i];
			}
		}
		if(r1.equalsIgnoreCase(r2)) {
			System.out.println("YES");
		}else {
			System.out.println("NO");
		}
	}
}
}
