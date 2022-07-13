# Matrix-multipliacation

import java.util.Scanner;

public class Main{

public static void main(String[] args) {
	
	Scanner sc = new Scanner(System.in);
	
	int[][] a = new  int[3][3];
	int[][] b = new  int[3][3];
	int[][] temp = new  int[3][3];
	
	int i,j;
	
	System.out.println("Enter your first matrix:");
	for(i = 0 ; i<3 ; i++) {
		
		for(j = 0 ; j<3 ; j++) {
			
			a[i][j] = sc.nextInt();
		}
	
	}
	
	System.out.println("Enter your second matrix:");
	for(i = 0 ; i<3 ; i++) {
		
		for(j = 0 ; j<3 ; j++) {
			
			b[i][j] = sc.nextInt();
		}
	
	}
	
	System.out.println("Your answer is:");
	for(i = 0 ; i<3 ; i++) {
		
		for(j = 0 ; j<3 ; j++) {
		    temp[i][j] = 0;
		    for(int k = 0 ; k<2 ; k++){
			temp[i][j] = temp[i][j] +a[i][k] * b[k][j];
		    }
		}
	}
	
	for(i = 0 ; i<3 ; i++) {
		for(j=0 ; j<3 ; j++) {
			
			System.out.print(temp[i][j]+" ");
			
		}
		
		System.out.println("  ");
	}
		
	
}
}
