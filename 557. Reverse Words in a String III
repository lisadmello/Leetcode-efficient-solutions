//TIME COMPLEXITY O(n)
public class Solution {
    public String reverseWords(String s) {
      // Split the string into individual words
        String[] words = s.split(" ");
      // Use String builder to create final answer
        StringBuilder answer =  new StringBuilder();
      // for each word
        for(int i=0;i<words.length;i++){
      // reverse the word and append to final answer
            answer.append(reverseWord(words[i]));
      // add a white space  
            answer.append(" ");
        }
      // return the trimmed string version of the final answer
        return answer.toString().trim();
        
    }
    
    public String reverseWord(String word){
      // if word length is zero return the word
        if(word.length()==0)
            return word;
       // convert string to character array
        char[] characters = word.toCharArray();
        // get length of the char array
        int l = characters.length;
        // swap all the characters until mid of the char array
        for(int j = 0; j<characters.length/2;j++){
            char temp = characters[j];
            characters[j] = characters[l-j-1];
            characters[l-j-1] = temp;
        }
        // return reversed version of the string
        return String.valueOf(characters);
    }
}
