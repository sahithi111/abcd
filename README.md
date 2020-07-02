# abcd_epam
import java.util.Scanner;

class MyCal{
    public static long power(int i,int j) throws Exception {
        if(i<0||j<0) {
            throw new Exception("n or p should not be negative.");      
        }
        else if(i==0&&j==0) {
            throw new Exception("n and p should not be zero.");
        }
        else {
            long result=(long)(Math.pow(i,j));
            return result;
        }
    }
    
}

public class Solution {
    public static final MyCal my_cal=new MyCal();
    public static final Scanner in=new Scanner(System.in);
    
    public static void main(String[] args) {
        while (in.hasNextInt()) {
            int i=in.nextInt();
            int j=in.nextInt();
            
            try {
                System.out.println(my_cal.power(n, p));
            } catch (Exception e) {
                System.out.println(e);
            }
        }
    }
}
