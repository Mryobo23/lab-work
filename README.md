
public class main {

	public static void main(String[] args) {
		
		x(5);
		
		// Calling the countEvenValues Method with @param limit = 5
		System.out.println("Number of Even Values from 0 to limit : " + countEvenValues(5));
	}
	
	public static void x(int y)
	{
		int z = 0;
		for(int i=0;i<=y;i++) 
		{
		if(i%2 == 0) {
			z++;
			}else 
			  {continue;
			}
		}
		System.out.println("Count = " + z);
	}
	
	
	public static int countEvenValues(int limit) {
		/*
		 	A method to count the number of even values from Zero to a specified Limit  
		 	@param limit : An integer value which will be used as the limit
		*/
		
		// Initializing Count with Zero
		int count = 0;
		
		// Looping from 0 to the limit passed in the parameter
		for (int number = 0; number <= limit; number++) {
			// Condition to check if the number is Even
			if(number%2 == 0) {
				// Add 1 to count variable if the number is even
				count++;
			}
			else {
				// Continue if the number is not even
				continue;
			}
		}
		// Returns the count of even values
		return count;
	}
}
