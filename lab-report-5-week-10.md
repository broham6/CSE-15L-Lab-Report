**Lab Report 5:**

*All differences have been found using the command `vimdiff`*

*Test 1:*
- 518.md: [foo *[bar [baz](/uri)](/uri)*](/uri)
- My repo output: []
- Class repo output: [/uri]
- The expected output is [/uri] with the working link being [baz](/uri), meaning my implementation is wrong. 
- The issue lies in my code's inability to handle complicated nested links. Improving the parsing for brackets and paranthesis should fix this issue. 

*Test 2:*
- 500.md: [link](#fragment)

[link](http://example.com#fragment)

[link](http://example.com?foo=3#frag)
- My repo output: []
- Class repo output:[#fragment, http://example.com#fragment, http://example.com?foo=3#frag]
- The expected output is the same as the class repo output.
- I'm not exactly sure the reason for this difference in outputs since these should be simple links, and when test my MarkdownParse file against these specific links, they work. Hence, it seems that this bug is caused by the running the case with the script somehow.
- ![markdownParse]()
