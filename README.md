# AssementSubmission
package day5;

import java.util.Scanner;

public class TaxCalculator {
	
	public static void main(String xyz[])
	   {		   
		   Scanner sc = new Scanner(System.in);
		   
		System.out.print("Enter Salary :- ");
		int salary = sc.nextInt();
	    float tax = 1;
		int taxRate = 0;
		float grossSal=0;	
	    float addSalary= salary+0.15f+0.60f;
	 
   System.out.println("Total salary+Incentives is" + addSalary);
	    
		if(addSalary<500000)
		{
			taxRate= 0;
			tax= (float)(addSalary * 0);
			grossSal=addSalary+tax;
		}
	    
	    
		else if( addSalary>500000 && addSalary<1000000)
		{
			taxRate = 20;
			tax = (float)(addSalary * 0.20);
			grossSal=addSalary+tax;
			
		}
		else if(addSalary>1000000)
		{
			taxRate = 30;
			tax = (float)(addSalary * 0.30);
			grossSal=addSalary+tax;
		}
		
		System.out.println("For Salary "+ addSalary + ", Tax would be @ "+ taxRate +"% tax amount =" + tax +" Rs. " );
		
		System.out.println("Total Gross monthly salary is = "+ grossSal);
		
	   }
	}


//output:-

Enter Salary :- 
5000000
Total salary+Incentives is5000000.5
For Salary 5000000.5, Tax would be @ 30% tax amount =1500000.1 Rs. 
Total Gross monthly salary is = 6500000.5

