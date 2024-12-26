import java.util.Scanner;

public class PalindromeChecker {
    public static boolean isPalindrome(String input) {
        // Convert to lowercase and remove non-alphanumeric characters
        String cleanedString = input.replaceAll("[^a-zA-Z0-9]", "").toLowerCase();
        
        // Two-pointer approach
        int left = 0;
        int right = cleanedString.length() - 1;
        
        while (left < right) {
            // Compare characters at left and right
            if (cleanedString.charAt(left) != cleanedString.charAt(right)) {
                return false; // Not a palindrome
            }
            // Move pointers towards the center
            left++;
            right--;
        }
        
        return true; // It's a palindrome
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        System.out.print("Enter a string to check if it's a palindrome: ");
        String userInput = scanner.nextLine();

        if (isPalindrome(userInput)) {
            System.out.println("\"" + userInput + "\" is a palindrome!");
        } else {
            System.out.println("\"" + userInput + "\" is not a palindrome.");
        }

        scanner.close();
    }
}
