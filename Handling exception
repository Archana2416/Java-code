package q28434;
import java.io.*;
import java.util.*;

public class WordFrequencyAnalyzer {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        
        // Read the file name from standard input
        String fileName = scanner.nextLine().trim();
        scanner.close();
        
        // TreeMap keeps the words automatically sorted in alphabetical order
        TreeMap<String, Integer> wordCounts = new TreeMap<>();
        
        try (BufferedReader br = new BufferedReader(new FileReader(fileName))) {
            String line;
            
            // Read the file line by line
            while ((line = br.readLine()) != null) {
                // Split lines into words by whitespace
                String[] words = line.split("\\s+");
                
                for (String word : words) {
                    if (!word.isEmpty()) {
                        // Convert words to lowercase for case-insensitive counting/sorting
                        String cleanWord = word.toLowerCase();
                        wordCounts.put(cleanWord, wordCounts.getOrDefault(cleanWord, 0) + 1);
                    }
                }
            }
            
            // Print out each lowercase word and its frequency
            for (Map.Entry<String, Integer> entry : wordCounts.entrySet()) {
                System.out.println(entry.getKey() + ": " + entry.getValue());
            }
            
        } catch (FileNotFoundException e) {
            // Print error with println to include a trailing newline character
            System.out.println("File does not exist");
        } catch (IOException e) {
            e.printStackTrace();
        }
    }

}
