# PalindromeCheckerApp
import java.util.Scanner;

public class PalindromeCheckerUC3 {
    public static void main(String[] args) {

        Scanner scanner = new Scanner(System.in);

        // Get input from user
        System.out.print("Enter a string: ");
        String original = scanner.nextLine();

        String reversed = "";

        // Reverse string using for loop
        for (int i = original.length() - 1; i >= 0; i--) {
            reversed = reversed + original.charAt(i); // String concatenation
        }

        // Compare original and reversed string
        if (original.equals(reversed)) {
            System.out.println("The string is a Palindrome.");
        } else {
            System.out.println("The string is NOT a Palindrome.");
        }

        scanner.close();
    }
}
