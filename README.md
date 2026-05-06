# Class_Assignment-
class Solution {
    public int sumOfTheDigitsOfHarshadNumber(int x) {
        int sum = 0;          
        int temp = x;         
        // Loop 
        while (temp > 0) {
            sum += temp % 10; 
            temp /= 10;       
        }
        // Check 
         return (x % sum == 0) ? sum : -1;
    }
}
