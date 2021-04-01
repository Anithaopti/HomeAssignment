# HomeAssignment
package Week3;
import java.util.LinkedHashSet;
import java.util.Set;
public class RemoveDup {
    public static void main(String[] args) {
      
          String str = "PayPal India";
          char[] ch = str.toCharArray();
        
        Set<Character> charSet = new LinkedHashSet<Character>();
        Set<Character> dupCharSet = new LinkedHashSet<Character>();
        for (Character eachChar : ch) {
            if (!charSet.add(eachChar)) {
                dupCharSet.add(eachChar);
            }
        }
         charSet.removeAll(dupCharSet);
        System.out.println("Charset");
        for (Character eachCh : charSet) {
            if(eachCh!=' ')
                System.out.println(eachCh);
        }
    }
}
