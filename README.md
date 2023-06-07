# Number_Guessing_game
I develop this project using Java and used Object Oriented concept class, method and object.
import javax.swing.*;
import java.util.*;
class number{
    void guess(){
        Random rand = new Random();
        int num = rand.nextInt(100); 
        Scanner sc = new Scanner(System.in);
        System.out.println("****************************************\nYOU HAVE ONLY 10 ATTEMPTS\n****************************************");

        int inputnum;
        for(int i=0;i<=10;i++){
        System.out.println("********************\nGuess a number between 1 to 100\n********************");
        inputnum = sc.nextInt();

            if(inputnum>num){
                System.out.println("Input number is greater");
            }
            else if(inputnum<num){
                System.out.println("Input number is smaller");
            }
            else{
                System.out.println("Congratulations you find the number \n You scored: "+i);
            }
        }
    }
}
class guess{
    public static void main(String[] args) {
        number ref = new number();
        ref.guess();
    }
}
