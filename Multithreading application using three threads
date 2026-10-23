import java.util.InputMismatchException;
import java.util.Scanner;

public class ExceptionHandlingExample {
    public static void main(String[] args) {
        Scanner input = new Scanner(System.in);
        int a, b;

        try {
		System.out.print("Enter the value of 'a': ");
		a = input.nextInt();
		System.out.print("Enter the value of 'b': ");
		b = input.nextInt();
		System.out.println("Result of a/b: " + divide(a, b));
        } catch (ArithmeticException e) { 
            System.out.println("Arithmetic Exception: " + e.getMessage());
        } catch (InputMismatchException e) { // Complete the code...
            System.out.println("Input Mismatch Exception: Please enter valid integer values.");
        }

        input.close();
    }

    public static int divide(int a, int b) {
        return a / b;
    }
}
