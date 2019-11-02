# arsheed
import java.util.LinkedList;
import java.util.Queue;
import java.util.Scanner;


public class QueueProble 
{
   public static void main(String[] args) 
   {
	   Scanner sc=new Scanner(System.in);
	         int n=sc.nextInt();
	         Queue<Integer> q=new LinkedList();
	         int a2[]=new int [n];//Ideal Order
	   for(int i=0;i<n;i++)
	   {
		  q.add(sc.nextInt());
	   }
	   
	   for(int i=0;i<n;i++)
	   {
		a2[i]=sc.nextInt();
	   }
	       int time=0,k=0;
	       while(q.isEmpty()!=true) {
	    	   if(q.peek()==a2[k]) {
	    		   q.remove(q.peek());time++;k++;
	    	   }else {
	    		   int h=q.peek();
	    		   q.remove(q.peek());
	    		   q.add(h);time++;
	    	   }
	       }
	
	  System.out.println(time);
   }
}
