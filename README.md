# school-work1
import java.util.Scanner;

public class problem2019 {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		Scanner scan=new Scanner(System.in);
		while(scan.hasNext()) {
			int n=scan.nextInt();
			int m=scan.nextInt();
			if(m==0&&n==0)
				break;
			int []a=new int[n+1];int i=0;
			for(;i<n+1;i++) {
				int b =scan.nextInt();
				if (b<m) {
					a[i]=b;
				}
				else {
					a[i]=m;
					a[i+1]=b;
					i++;
					break;
				}
				
			}for(int j=i;j<n+1;j++)
					a[j]=scan.nextInt();
			for(int j=0;j<n+1;j++)
				if(j<n)
				System.out.print(a[j]+" ");
				else
					System.out.println(a[j]);
		}
	}
}
