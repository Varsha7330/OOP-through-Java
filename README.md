# OOP-through-Java
import java.util.Scanner;
public class LinearSearch {
	public static void main(String args[]) {
	Scanner sc=new Scanner(System.in);
	System.out.println("enter n value: ");
	int n=sc.nextInt();
	int A[]=new int[n];
	System.out.println("enter array elements: ");
	for(int i=0;i<n;i++) {
	A[i]=sc.nextInt();
	}
	System.out.println("enter key value: ");
	int key=sc.nextInt();
	int result=linear(A,key);
	if(result== -1) {
		System.out.println("element not found: ");
	}
	else{
		System.out.println("element found at index "+result );
	}
	sc.close();
	}
	public static int linear(int A[],int key) {
		for(int i=0;i<A.length;i++) {
			if(A[i]==key) {
			return i;
			}
	}
	return -1;
	}
}


	
