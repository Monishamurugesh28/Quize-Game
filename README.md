# Quize-Game

package quizegame;
import java.util.Scanner;
public class Quizegame {
private static final Scanner sc = null;

public static void main(String [] args) {
	int score=0;
	System.out.println("------welcome to the game------");
String []questions= {"1).who is the cm of TN?"," 2).what is the capital of india?","3).which company developed java?"," 4).What is 10+20?","5).which lang is used for android development?"};
String [][]options={{"a)stalin","b)palaniswamy","c)joseph vijay"},{"a)mumbai","b)delhi","c)chennai"},{"a)microsoft","b)Apple","c)google"},{"a)30","b)50","c)90"},{"a)python","b)java","c)C"}};
char[] Answers= {'c','b','a','a','b'};
for(int i=0;i<questions.length;i++) {
	System.out.println();
	System.out.println(questions[i]);

for(int j=0;j<options[i].length;j++) {
	System.out.println();
	System.out.println(options[i][j]);
}
Scanner sc=new Scanner(System.in);
System.out.print("Enter your answer: ");
char userAnswer = sc.next().charAt(0);
if(userAnswer == Answers[i]){
    System.out.println(" your Answer is  Correct !");
    score++;
} 
else {
    System.out.println(" your Answer is Wrong! ");
}
}

System.out.println();
System.out.println("********QUIZ COMPLETED*********");
System.out.println("Your Score: " + score + "/" + questions.length);
if (score == 5) {
System.out.println("Excellent!");
} 
else if (score >= 3) {
System.out.println("Good Job !");
} 
else {
System.out.println(" Next Time Better Luck !");
}

sc.close();

}
}



