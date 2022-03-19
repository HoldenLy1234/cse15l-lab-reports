# Lab Report #5
For this lab I will be reviewing my own markdown parse: [My MarkdownParse](https://github.com/HoldenLy1234/markdown-parse)

The other file I will be reviewing is the week 9 MarkdownParse my group did.

# Finding differences
I found differences using the diff command, I used it to find the differences between my two outputs in a new file. I then looked through the new file output to manually look for two markdown files, which I found were 201.md, and 496.md.

# Markdown 201
My MarkdownParse output for markdown201.md was this
```
[]
```
the output for Week 9's Markdownparse was
```
[baz]
```
The correct answer that I found in the preview is 

![correct](https://i.imgur.com/yUOmgkd.png)

Meaning that there are no links, meaning that there should be a blank space. My markdownparse produced this, but the week 9 markdown didnt. I believe however, both are incorrect, but I will be reviewing Week 9's markdown parse.

The issue in the code lies within here

![incorrect](https://i.imgur.com/8AlkbwB.png)
The code doesn't check whether or not there is something between end bracket and the next open parenthesis. This causes it to recognize baz as a link when it shouldnt actually be a link.You would need to check for a parenthesis directly after a close bracket to fix this, but it would be an awkward fix.

# Markdown 496

My MarkdownParse output for markdown496.md was this
```
[link]
```
the output for Week 9's Markdownparse was
```
[]
```
Using a preview, the correct code was this

![correct](https://i.imgur.com/S1xxpAj.png)

Meaning that there are also no links in this one, however the markdown parse from week 9 produced this, but my own markdown parse read it as a link. I think this is because my code doesn't account for multiple parenthesis during the actual coding. The issue can be found here.

![incorrect](https://i.imgur.com/Vd4lmHX.png)

The fix would be to add a line that accounts for multiple parenthesis, or it checks for each one and then reads the entire thing as plain text to count how many parenthesis there actually are to see if it should be just plaintext inbetween the two parenthesis.