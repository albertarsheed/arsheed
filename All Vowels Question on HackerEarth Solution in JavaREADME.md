# arsheed
import java.util.Scanner;
import java.util.TreeSet;


public class AreAllCharactersVowels {
public static void main(String[] args) {
	Scanner sc=new Scanner(System.in);
	int n=sc.nextInt();sc.nextLine();
	String s=sc.nextLine().trim();
	TreeSet<Character>tr=new TreeSet();
	for(int i=0;i<n;i++) {
		if(s.charAt(i)=='a'||s.charAt(i)=='e'||s.charAt(i)=='i'||s.charAt(i)=='o'||s.charAt(i)=='u') {
			tr.add(s.charAt(i));
		}
	}
	if(tr.size()==5) {
		System.out.println("YES");
	}else {
	System.out.println("NO");
	}
}
}
/*
Another Method With Lesser Time Complexity

*/
import java.util.Scanner;
import java.util.TreeSet;


public class AreAllCharactersVowels {
public static void main(String[] args) {
	Scanner sc=new Scanner(System.in);
	int n=sc.nextInt();sc.nextLine();
	String s=sc.nextLine().trim();
	int a[]=new int[26];
	for(int i=0;i<n;i++) {
		a[s.charAt(i)-97]++;
	}
	if(a[0] >=1 && a[4]>=1 && a[8]>=1 && a[14]>=1 && a[20]>=1) {
		System.out.println("YES");
	}else {
		System.out.println("NO");
	}
}
}
