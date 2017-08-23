    package combinatorics;

    import java.util.*;
    import java.math.*;

    public class Combinatorics { 
    //Combinatorics Class
    //Cominatorics defined: A branch or mathematics that studies finite discrete structures.
    //1: factorial method: n! is used to count the number of ways to arrange n distinct objects into a sequence.
    //2: permutations method: an ordered arrangement of a set of N objects taken n at a time.
      
        //1
        public static BigInteger factorial(int n){
          BigInteger number = BigInteger.ONE;
            for(int i = 1; i <= n; i++){
              number = number.multiply(new BigInteger(i + ""));
            }
            return number;
        }
        
        //2
        public static BigInteger permutations(int N, int n){
          BigInteger number = BigInteger.ONE;
            for(int i = (N - n) + 1; i <= N; i++){
              number = number.multiply(new BigInteger(i + ""));
            }
        return number;   
        }
      }

