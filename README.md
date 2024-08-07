
java
public class StringExample {
    public static void main(String[] args) {
       
        String str1 = "Hello";
        String str2 = new String("World");

      
        System.out.println("Length of str1: " + str1.length());

       
        String str3 = str1 + " " + str2;
        System.out.println("Concatenated string: " + str3);

        
        System.out.println("Character at index 1 in str1: " + str1.charAt(1));

     
        System.out.println("Substring of str3 from index 6 to 11: " + str3.substring(6, 11));

      
        System.out.println("str1 in uppercase: " + str1.toUpperCase());
        System.out.println("str2 in lowercase: " + str2.toLowerCase());

       
        System.out.println("Replace 'l' with 'p' in str1: " + str1.replace('l', 'p'));

        
        String str4 = "Hello";
        System.out.println("str1 equals str4: " + str1.equals(str4));
        System.out.println("str1 equalsIgnoreCase str2: " + str1.equalsIgnoreCase("HELLO"));

      
        System.out.println("Index of 'l' in str1: " + str1.indexOf('l'));
        System.out.println("Index of 'World' in str3: " + str3.indexOf("World"));

       
        String[] words = str3.split(" ");
        System.out.println("Words in str3:");
        for (String word : words) {
            System.out.println(word);
        }

        StringBuilder sb = new StringBuilder();
        sb.append(str1);
        sb.append(" ");
        sb.append(str2);
        System.out.println("StringBuilder content: " + sb.toString());

       
        char[] charArray = str1.toCharArray();
        System.out.println("Characters in str1:");
        for (char c : charArray) {
            System.out.println(c);
        }
    }
}
