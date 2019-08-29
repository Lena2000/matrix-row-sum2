# matrix-row-sum2
Ввод/вывод элементов матрицы и вывод суммы элементов каждой строки напротив этой строки
package двумер4;

import java.util.Scanner;

/**
 *
 * @author LENOVO
 */
public class Двумер4 {

    /**
     * @param args the command line arguments
     */
   public static void main(String[] args) {
          Scanner sc=new Scanner(System.in);
          System.out.println("Введите размер высоты матрицы:");
          int n=sc.nextInt();
          System.out.println("Введите размер ширины матрицы:");
          int m=sc.nextInt();
          int k=n*m;
          System.out.println("Введите "+k+" элементов матрицы:");
          int mas[][]=new int[n][m];
          int i;
          int j;
          for(i=0; i<n; i++){
              for(j=0;j<m ;j++){
               mas[i][j]=sc.nextInt();
              }
          }
          int sum;
          System.out.println("Ваши элементы матрицы:");
          for(i=0; i<mas.length; i++){
              sum=0;
          for(j=0; j<mas[i].length; j++){
               sum=sum+mas[i][j];
              System.out.print(mas[i][j]+ "\t");  
              
          }
          
          
           System.out.println("Сумма строки - "+ sum );
              System.out.println();
          }
          
          
          
          
    }
} 
