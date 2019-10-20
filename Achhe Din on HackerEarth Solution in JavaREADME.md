# arsheed

import java.io.BufferedReader;
import java.io.InputStreamReader;
import java.util.*;
public class TestClass1 {
    public static void main(String args[] ) throws Exception {
       
        BufferedReader br = new BufferedReader(new InputStreamReader(System.in));
       int t=Integer.parseInt(br.readLine().trim());
       while(t-->0){
            int n=Integer.parseInt(br.readLine().trim());
            String s[]=br.readLine().split(" ");
            HashMap<Integer,Integer> hs=new HashMap();
            int a[]=new int[n];
            for(int i=0;i<n;i++){
                a[i]=Integer.parseInt(s[i]);
                if(hs.get(a[i])==null){
                    hs.put(a[i],1);
                }else{
                    hs.put(a[i],hs.get(a[i])+1);
                }
            }
            Set <Integer>ss=hs.keySet();
            for(Integer ai:ss) {
            	if(hs.get(ai)==1) {
            	System.out.println(ai);break;}
            }
       }

    }
}
