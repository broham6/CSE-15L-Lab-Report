**Lab Report 2:**

* Bug 1 (lab 3): I made a [test-file](https://github.com/broham6/markdown-parse/blob/7d0bcc8c297db6f6afbab1a5617037147b82576e/breaking-test.md) with no parentheses.
* Symptom: The program searchs for the parentheses but doesn't find any, resulting in a IndexOutOfBoundsException being thrown.
* Console output: 
        Exception in thread "main" java.lang.StringIndexOutOfBoundsException: begin 0, end -1, length 6
        at java.base/java.lang.String.checkBoundsBeginEnd(String.java:3751)
        at java.base/java.lang.String.substring(String.java:1907)
        at MarkdownParse.getLinks(MarkdownParse.java:20)
        at MarkdownParse.main(MarkdownParse.java:37)
 * Fix: Added a try and catch statement that would print out an error message telling the user that the markdown file is using the incorrect format - !
 
 
        
Bug 2 (lab 3): Parantheses in the middle of link; symptom: Incorrect output; console output:
[parantheses-in-the-middle(, link.html]
        
Error for bug 3 (lab 4): 
