import java.util.Scanner;

public class WordCount {
public static void main (String[] args) {
	Scanner scanner = new Scanner(System.in);
	System.out.println("Enter the text:");
	String text = scanner.nextLine();

	text = text.trim();
	int count = 0;
	if(!text.isEmpty()) {
		String[]words = text.split("\\s+");
		count = words.length;
	}
	System.out.println("Number of words in the text:"+ count);
	scanner.close();
}
}
