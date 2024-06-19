import java.util.*;
class arrayadd{
    arrayadd(int[][] arr1,int[][] arr2,int r,int c){
        int[][] arr3=new int[r][c];
        for (int i=0;i<arr3.length;i++){
            for (int j=0;j<arr3[i].length;j++){
                arr3[i][j]=arr2[i][j]+arr1[i][j];
            }
        }
        for (int i=0;i<arr3.length;i++){
            for (int j=0;j<arr3[i].length;j++){
                System.out.print(arr3[i][j]+"  ");
            }
            System.out.println(" ");
        }


    }
}
public class additionofarray {
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        System.out.println("Matrices dimensions should be same ! ");
        System.out.print("Enter rows : ");
        int r=sc.nextInt();
        System.out.print("Enter columns : ");
        int c=sc.nextInt();
        int [][] arr1=new int[r][c];
        System.out.println("Enter "+(r*c)+" elements in array 1 -------- ");
        for (int i=0;i<arr1.length;i++){
            for (int j=0;j<arr1[i].length;j++){
                arr1[i][j]=sc.nextInt();
            }
        }
        int [][] arr2=new int[r][c];
        System.out.println("Enter "+(r*c)+" elements in array 2 -------- ");
        for (int i=0;i<arr2.length;i++){

            for (int j=0;j<arr2[i].length;j++){
                arr2[i][j]=sc.nextInt();
            }
        }
        arrayadd obj=new arrayadd(arr1,arr2,r,c);
    }
}
