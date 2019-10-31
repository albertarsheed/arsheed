# arsheed
import java.util.*;

public class CheckIfDoubleString {
   public static void main(String[] args) {
	  Scanner sc=new Scanner(System.in);
	  int t=sc.nextInt();sc.nextLine();
	  while(t-->0) {
		  String s=sc.next();
		 if(s.length()==1 ||(s.length()==2 && s.charAt(0)!=s.charAt(1))) {
			 System.out.println("No");
		 }
		 else if(s.length()==2 &&(s.charAt(0)==s.charAt(1))) {
			 System.out.println("Yes");
		 }
		 else {
			 TreeSet<Character>tr=new TreeSet();
			 char c[]=s.toCharArray();
		     for(int i=0;i<c.length;i++) {
		    	 tr.add(c[i]);
		     }
		     if(tr.size()==s.length()) {
		    	 System.out.println("No");
		     }else {
		    	 System.out.println("Yes");
		     }
		 }
		 
		 
	  }

  
   }
   
   
}
