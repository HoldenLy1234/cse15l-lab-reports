## Lab Report #4 

Link to my repository: [My Repository](https://github.com/HoldenLy1234/markdown-parse)
Link to other repository from week 7[Lab Repository](https://github.com/jdweak/markdown-parse/blob/main/MarkdownParse.java)
I will be running 3 tests and seeing how both repositories/MarkdownParse files run the tests presented by the 3 snippets.
This is the markdown parse test file I will be using, then I will be running them through JUnit Tests.
![MDTest](https://i.imgur.com/rAOluco.png)

## Snippet #1
I used commonmark to see what it should return,and it returns this
![snippet1](https://i.imgur.com/wLAQN7J.png)

This means that the only link that should be returned is %60google.com

For my repository it returned

![myrepos1](https://i.imgur.com/ECdVY9P.png)

For the test repository it returned

![week7repos1](https://i.imgur.com/rNkIkRb.png)

## Snippet 2
I used commonmark to see what it should return,and it returns this
![snippet2](https://i.imgur.com/Wq26MDZ.png)

This means that the links that should be returned are a.com, a.com(()), and example.com

For my repository it returned

![myrepos2](https://i.imgur.com/dnd46N7.png)

For the test repository it returned

![week7repos2](https://i.imgur.com/5KZ6HzL.png)

## Snippet 3
I used commonmark to see what it should return,and it returns this
![snippet3](https://i.imgur.com/9eCF6tS.png)

This means that the link that should be returned is "https://ucsd-cse15l-w22.github.io/" 

For my repository it returned

![myrepos3](https://i.imgur.com/8M88jLC.png)

For the test repository it returned

![week7repos3](https://i.imgur.com/vKSocA6.png)

## Questions

Question 1: I think that for snippet one for my markdown parse it would be a much more involved change, however with the week 7's markdownparse I compared it to, it would maybe be around 8-10 lines, so it could be a small change, this is because I would have to add many more lines for mine due to how it is not completely set up to run different types of checks, I think this is just checking for backticks, so it might be a smaller change.

Question 2: I think that this is a much more involved change for both my MarkdownParse, and the one I compared it to, due to the fact that you are dealing with nested parenthesis, and also have to deal with escaped brackets.

Question 3: For the third snippet, it is also an involved change, I think that for my code, I would have to add many lines to deal with all the line breaks, I think that the other markdownparse could have less lines to make it, but it would still be an involved change.

