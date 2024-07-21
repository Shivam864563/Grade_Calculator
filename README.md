# Grade_Calculator

// Task 2) Student Grade Calculated System . 

import java.util.Scanner;
public class GradeCaluculate {
    
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in) ;
        
        System.out.println("Welcome To Student Grade Calculator System ....") ;
        System.out.println("Enter your Marks out of 100 in each subject !!!") ;
        System.out.println() ;
       
       System.out.print("Enter your Math Marks: ") ;
       int math = sc.nextInt() ;
       System.out.printf("You get %d Marks in Math Out of 100 ." , math) ;
       System.out.println() ;
       System.out.println() ;
       
        
       System.out.print("Enter your English Marks: ") ;
       int English = sc.nextInt() ;
       System.out.printf("You will get %d Marks in English Out of 100 ." , English ) ;
       System.out.println() ;
       System.out.println() ;
       
       
       System.out.print("Enter your Science Marks: ") ;
       int Science = sc.nextInt() ;
       System.out.printf("You will get %d Marks in Science Out of 100 ." ,Science ) ;
       System.out.println() ;
       System.out.println() ;
       
       System.out.print("Enter your ComputerScience Marks: ") ;
       int ComputerScience = sc.nextInt() ;
       System.out.printf("You will get %d Marks in ComputerScience Out of 100 ." , ComputerScience ) ;
       System.out.println() ;
       System.out.println() ;
       
       
       System.out.print("Enter your Hindi Marks: ") ;
       int Hindi  = sc.nextInt() ;
       System.out.printf("You will get %d Marks in Hindi Out of 100 ." , Hindi) ;
       System.out.println() ;
       System.out.println() ;
       
       // Sum of total marks calculate  .
       int TotalMarks =  math + English  + Science  + ComputerScience + Hindi ;
       float AveragePercentage  =   (float)(TotalMarks / 500.0 )*100 ;
       // Grade Calculation  .
        
      char  grade = 'P' ;
      if(AveragePercentage > 0) {
     if(AveragePercentage  <= 23 ){
        grade = 'F' ;
     }else if(AveragePercentage > 23 && AveragePercentage <= 50){
        grade = 'C' ;
     }else if(AveragePercentage >51 && AveragePercentage <=79){
        grade = 'B';
     }else if (AveragePercentage > 80 && AveragePercentage <=90){
        grade = 'A' ;
     } else {
        grade = 'O' ;
     }
      } 
    
      
     switch(grade) {
         case 'F' :
           System.out.printf("Your Toatal Marks is %d out of 500 , Average Percentage is %.2f , Grade is %c. %n" , TotalMarks,  AveragePercentage , grade) ;
           break ;
        case  'C' :
            System.out.printf("Your Toatal Marks is %d out of 500 , AveragePercentage is %.2f , Grade is %c. %n" , TotalMarks,  AveragePercentage , grade) ; 
             break ;
        case 'B':
          System.out.printf("Your Toatal Marks is %d out of 500 ,  AveragePercentage is %.2f , Grade is %c. %n" , TotalMarks, AveragePercentage , grade) ;    
              break ;
        case  'A':
         System.out.printf("Your Toatal Marks is %d out of 500 ,  AveragePercentage is %.2f , Grade is %c. %n" , TotalMarks,  AveragePercentage , grade) ;
            break ;   
            
        case  'O' :
           System.out.printf("Your Toatal Marks is %d out of 500 ,  AveragePercentage is %.2f , Grade is %c. %n" , TotalMarks,  AveragePercentage , grade) ;    
              break ;
              
        default :
        System.out.println("You have enter wrong Marks So Your data can't be Loded !!!") ;
     } 
     System.out.println() ;
     System.out.println("Thank You For Choosing the Student Grade Calculator ....");
    }
    
}
