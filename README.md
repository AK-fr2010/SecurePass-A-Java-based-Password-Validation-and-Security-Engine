# SecurePass-A-Java-based-Password-Validation-and-Security-Engine

import java.util.Scanner;
public class Main {
    public  static void main(String[]args) {
        Scanner scanner = new Scanner(System.in);

        System.out.print("(Note-> Password Should contain Atleast 8 characters , 1 special Character and Should not contain Any spaces ) \nPlease Enter Your Desired Password : ");
        String password = scanner.nextLine().trim();
        int length = password.length();

        if (length >= 8) {

            String rePassword ;
            if (password.contains(" ")) {
                System.out.println("Password Can't Contain Any Spaces ");
            } else if (password.contains(":")) {
                System.out.println("Password Can't Contain Any : ");
            } else if (password.contains(";")) {
                System.out.println("Password Can't Contain Any ; ");
            } else if (password.contains("{")) {
                System.out.println("Password Can't Contain Any { ");
            } else if (password.contains("}")) {
                System.out.println("Password Can't Contain Any } ");
            } else if (password.contains("[")) {
                System.out.println("Password Can't Contain Any [ ");
            } else if (password.contains("]")) {
                System.out.println("Password Can't Contain Any ] ");
            } else if (password.contains("=")) {
                System.out.println("Password Can't Contain Any = ");
            } else if (password.contains("+")) {
                System.out.println("Password Can't Contain Any + ");
            } else if (password.contains(")")) {
                System.out.println("Password Can't Contain Any ) ");
            } else if (password.contains("(")) {
                System.out.println("Password Can't Contain Any ( ");
            } else if (password.contains("^")) {
                System.out.println("Password Can't Contain Any ^ ");
            } else if (password.contains("%")) {
                System.out.println("Password Can't Contain Any % ");
            } else if (password.contains("!")) {
                System.out.println("Password Can't Contain Any ! ");
            } else if (password.contains("`")) {
                System.out.println("Password Can't Contain Any ` ");
            } else if (password.contains("~")) {
                System.out.println("Password Can't Contain Any ~ ");
            } else if (password.contains("|")) {
                System.out.println("Password Can't Contain Any | ");
            } else if (password.contains("'")) {
                System.out.println("Password Can't Contain Any ' ");
            } else if (password.contains(">")) {
                System.out.println("Password Can't Contain Any > ");
            } else if (password.contains("<")) {
                System.out.println("Password Can't Contain Any < ");
            } else if (password.contains(",")) {
                System.out.println("Password Can't Contain Any , ");
            } else if (password.contains("?")) {
                System.out.println("Password Can't Contain Any ? ");
            } else if (password.contains("/")) {
                System.out.println("Password Can't Contain Any / ");
            } else {
                System.out.print("Please Re-Enter Your Password : ");
            } rePassword = scanner.nextLine().trim();

            if (password.equals(rePassword)){
                System.out.println("============================");
                System.out.println("Your Password Is Saved");
                System.out.println("============================");
            }
            else {
                System.out.println("Error : The password DOESN'T match .");
            }


        }
        else {
            System.out.println("Please Ensure Your Password Has atleast 8 characters .");
        }

The code is really extensive as I currently learning about Java and not know very much but yeah it works so...... :)



        scanner.close();
    }
}
