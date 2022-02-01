# Lab Report #2

# Code change #1
## ![code change #1](https://i.imgur.com/fE1xmXn.png)
[File with failed input#1](https://github.com/HoldenLy1234/markdown-parse/blob/main/breaking.md)

## ![picture of it failing](https://i.imgur.com/IKC4GA8.png)

The failure is that the program doesn't account for there not being a closed bracket, so it won't account for there being a -1 in the ending length, and it'll return a a string out of bounds error. This is a bug, it is a coding error.

# Code change #2
## ![code change#2](https://i.imgur.com/3vLhfVt.png)
[File with failed input#2](https://github.com/HoldenLy1234/markdown-parse/blob/9aafa5f15d645d23f925cf016fd568b2cd5f32f6/breaking2.md)

## ![picture of failing](https://i.imgur.com/fntf39G.png)
The program can't find the first parenthesis, so it will run out of memory looking for the parenthesis. The lack of parenthesis in the input makes it so that the program will fail.

# Code change #3   
## ![code change#3](https://i.imgur.com/l9R3uNm.png)

[File with failed input#3](https://github.com/HoldenLy1234/markdown-parse/blob/main/breaking3.md)
## ![picture of failing](https://i.imgur.com/LaADE49.png)
It is not coded to read the the links as pictures, and will take the literal string instead. This is a coding error, and the failure of input was the ! that it doesnt take as an image.



