/*
 * To change this license header, choose License Headers in Project Properties.
 * To change this template file, choose Tools | Templates
 * and open the template in the editor.
 */
package testsimple;

/**
 *
 * @author Levit
 */
public class TestSimple {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        
        System.out.println("The highest value is "+getMaxValue());        
        //first let's get the highest number
        //let's get position for highest number
        //let's get the second highesr number not adjacent to the highest number +or-1
        //let's sum the two
    }
    
    public static int getMaxValue(){
        int maxVal = 0;//variable that will hold the maximum value
        int [] secArray;
        
        int[] theArray = new int[]{2, 26, 2, 23, 9, 22};//our array  
        
        int position = 0;
        
        int maxInArray1 = Integer.MIN_VALUE;//maximum value in the array   
        
        int hVal = 0;//highest value
        int sHVal = 0;//second highest value
       
          hVal = getHighestValue(theArray);
          sHVal = getsecondHighest(theArray, hVal, getArrayIndex(theArray, hVal));  
          
          
       System.out.println("Highest value is "+hVal+" second highest value is "+sHVal);
        
        final int sum = hVal+sHVal;
        return sum;
    }
    
    
    

//get second highest but keep asserting that they are not from position -1 or +1 of highest value
 public static int getsecondHighest(int[] input, int largVal, int largPos) {
            int largest,secondLargest;

            if(input[0] > input[1]) {
                largest = input[0];
                secondLargest = input[1];
            }
            else {
                largest = input[1];
                secondLargest = input[0];
            }

            for(int i = 2; i < input.length; i++) {
                if((input[i] <= largest) && input[i] > secondLargest && i!=largPos-1 && i!=largPos+1) {
                    secondLargest = input[i];
                }

                if(input[i] > largest && i!=largPos-1 && i!=largPos+1) {
                    secondLargest = largest;
                    largest = input[i];
                }
            }

            return secondLargest;
        }


    
    
    //got this from the internet ; how to get the integer position in an array
     public static int getArrayIndex(int[] arr,int value) {
        int k=0;
        for(int i=0;i<arr.length;i++){

            if(arr[i]==value){
                k=i;
                break;
            }
        }
    return k;
}
     //get the highest value is
  public static int getHighestValue(int[] numbers){
  int maxValue = numbers[0];
  for(int i=1;i < numbers.length;i++){
    if(numbers[i] > maxValue){
	  maxValue = numbers[i];
	}
  }
  return maxValue;
}
    
}
