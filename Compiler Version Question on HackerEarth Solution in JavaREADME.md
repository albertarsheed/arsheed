# arsheed
import java.util.Scanner;

public class PalindromicSequence {
    public static void main(String[] args) {
		Scanner sc=new Scanner(System.in);
	
			while(sc.hasNext()) {
				String s=sc.nextLine();
		     int i=0;
		     String r="";
		    for(i=0;i<s.length();) {
		    	if(s.charAt(i)=='/') {
		    		if((i+1)<s.length()&&s.charAt(i+1)=='/') {
		    	break;}else {
		    		r=r+s.charAt(i);
			    	 i+=1;
		    	}
		    	}
		    	else if(s.charAt(i)=='-') {
		    		if((i+1)<s.length()&&s.charAt(i+1)=='>') {
		    		 r=r+".";i+=2;}
		    		else {
		    			r=r+s.charAt(i);
				    	 i+=1;
		    		}
		    	 }else {
		    	 r=r+s.charAt(i);
		    	 i+=1;}
		     }if(i<s.length()) {
		     r=r+s.substring(i,s.length());}
		     System.out.println(r);
	}}
}
