import java.util.Scanner;

public class Mini_Project {

    public static void main(String[] args) {

        System.out.println(
                "**WELCOME TO MY GAME.**\n**WHENEVER YOU WANT TO EXIT THIS GAME JUST ENTER ANY NAGETIVE NUMBER!!**");

        int system_number = (int) (Math.random() * 100);

        Scanner sc = new Scanner(System.in);
        int user_number;
        do {
            System.out.print("Enter the correct number - ");
            user_number = sc.nextInt();

            if (user_number == system_number) {
                System.out.println("CONGRATULATIONS!!! YOU WON THE GAME.\n");
                System.out.println("!!THANKS TO PLAY THE GAME HOPE YOU ENJOY IT!!");
                break;
            } else if (user_number < system_number) {
                System.out.println("THE ENTERED NUMBER IS LESS THAN THE REQUIRED NUMBER");
            } else {
                System.out.println("THE ENTERED NUMBER IS GRETER THAN THE REQUIRED NUMBER");
            }

        } while (user_number > 0);

        System.out.println("THE ACTUAL NUMBER IS - " + system_number);
        System.out.println("!!THE GAME IS OVER!!");

    }
}
