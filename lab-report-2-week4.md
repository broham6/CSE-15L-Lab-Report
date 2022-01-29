**Lab Report 2:**

Error for bug 1 (lab 3): No paranthesis; symptom: Index out of bounds; console output: 
        Exception in thread "main" java.lang.StringIndexOutOfBoundsException: begin 0, end -1, length 6
        at java.base/java.lang.String.checkBoundsBeginEnd(String.java:3751)
        at java.base/java.lang.String.substring(String.java:1907)
        at MarkdownParse.getLinks(MarkdownParse.java:20)
        at MarkdownParse.main(MarkdownParse.java:37)
        
Error for bug 2 (lab 3): Extra closing paranthesis; symptom: Infinite loop; console output:
Exception in thread "main" java.lang.OutOfMemoryError: Java heap space
        at java.base/java.util.Arrays.copyOf(Arrays.java:3511)
        at java.base/java.util.Arrays.copyOf(Arrays.java:3480)
        at java.base/java.util.ArrayList.grow(ArrayList.java:237)
        at java.base/java.util.ArrayList.grow(ArrayList.java:244)
        at java.base/java.util.ArrayList.add(ArrayList.java:454)
        at java.base/java.util.ArrayList.add(ArrayList.java:467)
        at MarkdownParse.getLinks(MarkdownParse.java:20)
        at MarkdownParse.main(MarkdownParse.java:37)
        
Error for bug 3 (lab 4): 
