# 2Darray

1. Matrix Addition.

2.Matrix Multiplication.
// Online Java Compiler
// Use this editor to write, compile and run your Java code online
import java.util.Scanner;
class Main {
    static void inputMatrix(int[][] arr, int a, int b,Scanner sc){
        for(int i=0;i<a;i++){
            for(int j=0;j<b;j++){
               arr[i][j] = sc.nextInt();
            }
        }
    }
    static void printMatrix(int[][] arr,int r, int c){
        System.out.println("Entered matrix is");
        for(int i=0;i<r;i++){
            for(int j=0;j<c;j++){
               System.out.print(arr[i][j]+" ");
            }
            System.out.println();
        }
    }
    public static void main(String[] args) {
        Scanner sc= new Scanner(System.in);
        System.out.println("Enter the Matrix 1 dimensions");
        int r1=sc.nextInt();
        int c1=sc.nextInt();
        int[][] matrix_1 = new int[r1][c1];
        System.out.println("Enter the Matrix 1");
        inputMatrix(matrix_1,r1,c1,sc);
        printMatrix(matrix_1,r1,c1);
        System.out.println("Enter the Matrix 2 dimensions");
        int r2=sc.nextInt();
        int c2=sc.nextInt();
        int[][] matrix_2 = new int[r2][c2];
        System.out.println("Enter the Matrix 2");
        inputMatrix(matrix_2,r2,c2,sc);
        printMatrix(matrix_2,r2,c2);
        int[][] mult = new int[r1][c2];
    }
}
