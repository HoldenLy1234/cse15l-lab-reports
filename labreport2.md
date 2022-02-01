##Code change #1
![code change #1](https://imgur.com/a/E7545t4)
[link to fail test file](https://github.com/HoldenLy1234/markdown-parse/blob/main/breaking.md)
![picture of it failing](https://imgur.com/IKC4GA8)
The failure is that the program doesn't account for there not being a closed bracket, so it won't account for there being a -1 in the ending length, and it'll return a a string out of bounds error. This is a bug, it is a coding error.

##Code change #2
![code change#2](https://imgur.com/3vLhfVt)
[link to fail test file](https://github.com/HoldenLy1234/markdown-parse/blob/9aafa5f15d645d23f925cf016fd568b2cd5f32f6/breaking2.md)
![picture of failing](https://imgur.com/fntf39G)
The program can't find the first parenthesis, so it will run out of memory looking for the parenthesis. The lack of parenthesis in the input makes it so that the program will fail.

##Code change #3   
![code change#3](https://imgur.com/l9R3uNm)
[link to fail test file](https://github.com/HoldenLy1234/markdown-parse/blob/main/breaking3.md)
![picture of failing](https://imgur.com/LaADE49)
It is not coded to read the the links as pictures, and will take the literal string instead. This is a coding error, and the failure of input was the ! that it doesnt take as an image.



