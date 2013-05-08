random_number.
==============
import java.util.Arrays;


class Aleatorio {
    
  public static void main(String[] args) {
        numero numeroObject= new numero();
        int[] array = numeroObject.dedo();                    // obtain the array
        System.out.println(Arrays.toString(array));
	}
	
	
	
}

========================================================

import java.util.Random;

public class numero {
  
	public int[] dedo() {
		   Random diceRoller = new Random();
	        int[] cifra= new int[5];
	        int roll = diceRoller.nextInt(9) ;
            int i=0;
	        do {
	        	roll = diceRoller.nextInt(9);
	        	  if (roll != cifra[0] && roll != cifra[1] && roll != cifra[2] && roll != cifra[3] && roll != cifra[4]) {
	                  cifra[i] = roll;
	                  System.out.print(roll);
	                  i++;
	        	   }
	        }
	        	  while (i <= 4 );
	        
	        
	    
	        return cifra; 
	        
	}

}
	
