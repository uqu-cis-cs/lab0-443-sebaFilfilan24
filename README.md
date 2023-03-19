[![Open in Codespaces](https://classroom.github.com/assets/launch-codespace-f4981d0f882b2a3f0472912d15f9806d57e124e0fc890972558857b51b24a6f9.svg)](https://classroom.github.com/open-in-codespaces?assignment_repo_id=10523091)
# 443 - Lab 0 - Revision

Start working on the problem by reading and following the instructions in the comments in `App.java` file. 

## Using the command-line

Using the command-line in the Terminal, you can do the following: 

You can test your code by running the following command:

```bash
mvn clean test
```

You can run the program using the following command:
```bash
mvn clean compile exec:java
```

## Submitting your exam
You should use the following commands to submit your lab. Make sure that the current working directory is the repo's directory. 

```bash
git add src

git commit -m "a message"

git push
```
Replace `a message` with your own message! Do not simply copy and paste!

# Important!

You should only modify the `App.java` file, unless asked by the instructors to do additional modifications. 

Make sure that your code compiles and runs successfully. 

Make sure that your code passes all the tests before submission.



import static java.lang.System.in;
import java.util.Scanner;
public class ProjectGethub {

    public static void main(String[] args) {
        
         System.out.println( "Enter a number :");
         twisters();
         Scanner input = new Scanner(System.in);
         System.out.println( "Enter a String :");
         String str = input.nextLine();
         phoneKeypad (str);
    }
    
    public static void twisters() {
        
        for (int i=1 ; i<=110 ; i++){
        if ( i%2 == 0 ){
            System.out.println( "Tweetle");
        
            if (i%4==0)
                 System.out.println( "Beetle");
            
                if (i%6==0)
                    System.out.println("Poodle");
                } else {
                      System.out.println(" "+i+" ");
                }
            }
        }
    
    
    public static void phoneKeypad ( String str ) {
        String text =" ";
        for ( char letter : str.toUpperCase().toCharArray() ){
            switch (letter){
                case'A':
                case'B':  
                case'C': 
                    text+="2";
                    break;
                case'D':
                case'E':  
                case'F': 
                    text+="3";
                    break;    
                case'G':
                case'H':  
                case'I': 
                    text+="4";
                    break;   
                case'J':
                case'K':  
                case'L': 
                    text+="5";
                    break;    
                case'M':
                case'N':  
                case'O': 
                    text+="6";
                    break;    
                case'P':
                case'Q':  
                case'R':
                case'S':    
                    text+="7";
                    break;  
                case'T':
                case'U':  
                case'V': 
                    text+="8";
                    break; 
                case'W':
                case'X':  
                case'Y': 
                case'Z':    
                    text+="9";
                    break;    
            }
                    
        }System.out.println(text);
        
        
    } 
    
    
        
        
        
    

    
    
    
    
    
    
    
}
