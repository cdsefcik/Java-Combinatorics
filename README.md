#Java-Combinatorics

    package combinatorics;

    import java.util.*;
    import java.math.*;

    public class Combinatorics { 
    //Combinatorics Class
    //Cominatorics defined: A branch or mathematics that studies finite discrete structures.
    //factorial method: n! is used to count the number of ways to arrange n distinct objects into a sequence.
    
        public static BigInteger factorial(int n){
          BigInteger number = BigInteger.ONE;
            for(int i = 1; i <= n; i++){
              number = number.multiply(new BigInteger(i + ""));
            }
            return number;
        }
    }
