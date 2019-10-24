# arsheed
import java.util.HashMap;
import java.util.Scanner;

public class fdjsgfsjfhdgs {
public static void main(String[] args) {
	Scanner sc=new Scanner(System.in);
     int t=sc.nextInt();
     while(t-->0) {
    	 int n=sc.nextInt();
    	 HashMap<Integer,Integer> Rupam=new HashMap();
    	 int max1=0,max2=0;
    	 int a1=0,a2=0;
    	 for(int i=0;i<n;i++) {
    		 int a=sc.nextInt();
    		 if(Rupam.get(a)==null) {
    			 Rupam.put(a, 1);
    		 }else {
    			 Rupam.put(a,Rupam.get(a)+1);
    		 }
    		 if(Rupam.get(a)==max1 && a>a1) {
    			 a1=a;
    		 }
    		 if(Rupam.get(a)>max1) {
    			 max1=Rupam.get(a);
    			 a1=a;
    		 }
    		 
    		 
    	 }
    	 HashMap<Integer,Integer> Ankit=new HashMap();
    	 for(int i=0;i<n;i++) {
    		 int a=sc.nextInt();
    		 if(Ankit.get(a)==null) {
    			 Ankit.put(a, 1);
    		 }else {
    			 Ankit.put(a,Ankit.get(a)+1);
    		 }
    		 if(max2==Ankit.get(a) && a>a2) {
    			 a2=a;
    		 }
    		 if(Ankit.get(a)>max2) {
    			 max2=Ankit.get(a);
    			 a2=a;
    		 }
    	 }
    	 if(a1>a2) {
    		 System.out.println("Rupam");
    	 }else if(a2>a1){
    		 System.out.println("Ankit");
    	 }else {
    		 System.out.println("Tie");
    	 }
     }
}
}
