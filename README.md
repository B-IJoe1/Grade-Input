# Grade-Input
Users entering number scores in return for a grade average


    package lab02;

    public class ExFinal {


	  public static void main(String[] args) {

		Ex_Q1 A1=new Ex_Q1();
		A1.Gradeinput();
	}

    }


///////////////////////////////////////

    public static void Gradeinput()
    {
	  Scanner input = new Scanner(System.in);
	
	System.out.println("Please enter the first score");
	double score0=input.nextDouble();

	System.out.println("Please enter the second score");
	double score1=input.nextDouble();
	
	System.out.println("Please enter the third score");
	double score2=input.nextDouble();
	
	System.out.println("Please enter the fourth score");
	double score3=input.nextDouble();
	
	System.out.println("Please enter the fifth score");
	double score4=input.nextDouble();
	
	
	qualityPoints(score0,score1,score2, score3, score4);
  
    }

    public static void qualityPoints(double score0, double score1, double score2, double score3, double score4)
    {
    
  	if (score0 <= 60)
	  {
		System.out.println("Your grade is less than 60"); 
		System.out.println("0");
	  }
    
		if (score1>=60)
		{
			System.out.println("Your grade is greater than 60"); 
			System.out.println("1");
		}
		
	  if (score2>=70)
	  {
		System.out.println("Your grade is greater than 70 "); 
		System.out.println("2");
	  }
	
	 if (score3>=80)
	  {
		System.out.println("Your grade is greater than 80"); 
		System.out.println("3");
	  }
	
	if ( score4>=90)
	  {
		System.out.println("Your grade is greater than 90"); 
		System.out.println("4");
    }

	double average = (score0+score1+score2+score3+score4)/5;
	System.out.println("Your avereage is: "+ average); 

    }
