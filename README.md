Printing Pattern
In this program we’re going to code pyramid star pattern program . The logic of this program is this take any number input from user and store it in variable n and then run the for loop start from 0 to i start from j=n-i to j– and again take another for loop start from j=0 to j++ to print stars and after this take line changement statement after the end of main for loop 
Print Pyramid Star Pattern
Algorithm:
Enter the number as input from the user and store it in any variable.(‘n‘ in this case).
Run a loop ‘n’ number of times to iterate through each of the rows. From i=0 to i<n. The loop should be structured as for( i=0 ; i
 Run a nested loop inside the main loop to print the spaces before the pyramid. From j=n-i to j–. The loop should be structured as  for (int j=n-i; j>1; j–)
Inside this nested loop print white space System.out.print(” “); . 
Run another nested loop inside the main loop after the previous loop to print the stars in each column of a row. From j=0 to j<=i. The loop should be structured as for (int j=0; j<=i; j++ )
Inside this nested loop print star System.out.print(” *”); .
Move to the next line by printing a new line . System.out.println();
Code in Java:
import java.util.Scanner;
public class Pattern1 {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		System.out.println("Enter No");
		int n=sc.nextInt();
		 for (int i=0; i<n; i++) 
	        { 
	            for (int j=n-i; j>1; j--) 
	                System.out.print(" "); 
	            for (int j=0; j<=i; j++ ) 
	                System.out.print(" *"); 
	            System.out.println(); 
	        } 
	}

}
