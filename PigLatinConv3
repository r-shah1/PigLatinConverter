//PigLatinConv3.java
//converts a user entered English sentence into pig latin
//By Ruhul Shah

import java.util.Scanner;

public class PigLatinConv3 {
	static Scanner input = new Scanner(System.in);
	static String pigLatinSentence = "";
	
	public static void main(String[] args) {	
		System.out.println("Please enter English sentence: ");
		//define user input
		String eng_sentence = input.nextLine();
		//process sentence into individual tokens (words)
		String[] sentence_tokens = eng_sentence.split(" ");
		
		//run method printPigLatin on sentence tokens
		printPigLatin(sentence_tokens); 
		
		//display pig latin sentence
		System.out.println("Full Sentence: " + pigLatinSentence);
		
		}//end main

	//method to translate words into pig Latin and display
	public static void printPigLatin(String[] sentence_tokens) {
		for (String token : sentence_tokens) {
			StringBuilder sb_token = new StringBuilder(token); //change each token to string builder for mutator methods
			char ch = sb_token.charAt(0); //define character at first position of each word
			sb_token.deleteCharAt(0); //delete character at first position of each word
			sb_token.append(ch + "ay"); //append first character to end of each word and add "ay"
			
			pigLatinSentence += sb_token.append(" ");//combine pig latin words into sentence
			
			System.out.println("Each Word in Pig Latin: " + sb_token);
		}
	}//end method printPigLatin
	
}
