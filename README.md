//According to HSC Marks System
import java.util.*;
class  studentgradecalculator{
	public static void main(String []arg) {
		System.out.println("                          ACCORDING TO HSC MARKS SYSTEM");
		  System.out.println("____________________________________________________________________________________");
		System.out.println("Enter marks out of 100 for following subjects");
	    System.out.println("--------------------------------------------------------------------------------------");
		Scanner sc=new Scanner(System.in);
	    System.out.print("English: ");
	    int english=sc.nextInt();
	    System.out.print("Marathi: ");
	    int marathi=sc.nextInt();
	    System.out.print("Physics: ");
	    int physics=sc.nextInt();
	    System.out.print("Chemistry: ");
	    int chemistry=sc.nextInt();
	    System.out.print("Biology: ");
	    int biology=sc.nextInt();
	    System.out.print("Mathematics: ");
	    int math=sc.nextInt();
		if (english>100 || marathi>100 || physics>100 || chemistry>100 || biology>100 || math>100)
		{
			System.out.println("INVALID MARKS");
	    }
		else{
		int sum=english+marathi+physics+chemistry+biology+math; 
		System.out.println("Total of the marks is: "+sum );
		float percentage=(sum*100)/600;
		System.out.println("Percentage: "+percentage+"%");
		if (english>=35 && marathi>=35 && physics>=35 && chemistry>=35 && biology>=35 && math>=35 ){
		if (90<percentage && percentage<100){
			System.out.println("Remark: Outstanding");
		}
		else if (80<percentage && percentage<=90){
			System.out.println("Remark: Very Good ");
		}
		else if (70<percentage && percentage<=80){
			System.out.println("Remark: Good ");
		}
		else if (60<percentage && percentage<=70){
			System.out.println("Remark: Fair ");
		}
		else if (50<percentage && percentage<=60){
			System.out.println("Remark: Average ");
		}
		else if (40<percentage && percentage<=50){
			System.out.println("Remark: Below Average ");
		}
		else if (percentage>=35){
			System.out.println("Remark: Pass ");
		}
		else{
			System.out.println("Fail");
		    }
		}
	else{
		System.out.println("Fail");
		}
	}
}
}

