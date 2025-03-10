## Here are some Wildcards and Regex overview ##
~ __Wildcards are special character that represents one or more character in filenames or commands, allowing users to select multiple files at once.__
1) Asterisk ```*```: Matches any number of character, including none.  
 Example: ```*.txt``` matches all files ending with '.txt'.
2) Question Mark ```?```: Matches exactly one character or single character.  
Example: ```file?.txt``` matches ```file1.txt```, ```file2.txt```, etc.
3) Square Brackets ```[]```: Matches any one of the enclosed characters.  
Example: ```file[12].txt``` matches ```file1.txt``` and ```file2.txt```.
4) Curly Braces ```{}```:Matches a group of patterns.  
Example: ```file{1,2}.txt``` matches ```file1.txt``` and ```file2.txt```  

---
__Create 100 files like file1 file2...file100 and show only files__
- ```touch file{1..100}```
- ```ls file*```
- ```ls file file{1..100}``` 

__Delete 100 files like file1 file2...file100__
- ```rm file{1..100}```

__Find all the files with name ```_123``` (where_can be any character)__
- ```ls ?123```

__Find all the files whose name is exactly 4 character ex a123, test...__

- ```ls ????```
