# HCFLCM
CALCULATES HCF AND LCM
import java.util.Scanner;
public class KboatWords
{
    public static void main(String args[]) 
    {
        Scanner in = new Scanner(System.in);
        String names[] = new String[10];
        int l = names.length;
        System.out.println("Enter 10 names : ");
        
        for (int i = 0; i < l; i++) 
        {
            names[i] = in.nextLine();
        }
        
        System.out.println("Names that begin and end with letter A are:");

        for(int i = 0; i < l; i++)
        {
            String str = names[i];
            int len = str.length();
            char begin = Character.toUpperCase(str.charAt(0));
            char end = Character.toUpperCase(str.charAt(len - 1));
            if (begin == 'A' && end == 'A') 
            {
                System.out.println(str);
            }
        }
    }
}
class rectangle
{
    private int length,breadth;
    public rectangle(int l,int b)
    {
        length = l;
        breadth = b;
    }
    public rectangle()
    {
        length = 0;
        breadth = 0;
    }
    public int area()
    {
        int a = length*breadth;
        return a;
    }
    class Main
    {
        public static void main(String args[])
        {
            rectangle r1 = new rectangle(10,20);
            rectangle r2 = new rectangle();
            int ans = r1.area();
            System.out.println(ans);
            int s = r2.area();
            System.out.println(s);
        }
    }
}
