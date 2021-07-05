# zero-s-at-the-end
import java.util.*;
class program
{
    public static void reorder(int[] A)
    {
        int x = 0;
        for (int i: A)
        {
            if (i != 0) {
                A[x++] = i;
            }
        }
        for (int i = x; i < A.length; i++) {
            A[i] = 0;
        }
    }
 
    public static void main(String[] args)
    {
        int[] A = { 0,4,8,1,7,0,6,2};
         reorder(A);
        System.out.println(Arrays.toString(A));
    }
}
