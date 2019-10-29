# arsheed
import java.io.BufferedReader;
import java.io.IOException;
import java.io.InputStreamReader;
import java.util.*;

public class NonDuplicateElementFinding {
public static void main(String[] args) throws IOException {
	BufferedReader bf=new BufferedReader(new InputStreamReader(System.in));
	String s=bf.readLine();
	char c[]=s.toCharArray();
	Arrays.sort(c);
	HashMap<Character,Integer> hm=new HashMap();
	for(int i=0;i<c.length;i++) {
	if(hm.get(c[i])==null) {
		hm.put(c[i], 1);
	}else {
		hm.put(c[i],hm.get(c[i])+1);
	}
	}
  Set<Character> d=hm.keySet();
  int g=0;
  char e='d';
  for(Character f:d) {
	if(hm.get(f)>g) {
		g=hm.get(f);
		e=f;
	}
  }
	System.out.println(e+" "+g);
}
}
