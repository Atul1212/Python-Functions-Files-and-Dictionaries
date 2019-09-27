# Python-Functions-Files-and-Dictionaries
week 1 assigment
1>The textfile, travel_plans.txt, contains the summer travel plans for someone with some commentary. Find the total number of characters in the file and save to the variable num.
program:-
   
                fileref = open("travel_plans.txt","r")
                num = 0
                for i in fileref:
                      num += len(i)
                fileref.close()



2>We have provided a file called emotion_words.txt that contains lines of words that describe emotions. Find the total number of words in the file and assign this value to the variable num_words.
 programme:-  
 
         fileref = open("emotion_words.txt","r")
num_words = 0
for line in fileref:
    num_words += len(line.split())
fileref.close()



3>Assign to the variable num_lines the number of lines in the file school_prompt.txt.
programe:-
  
  num_lines = sum(1 for line in open('school_prompt.txt'))
   
   
  
  
4>Assign the first 30 characters of school_prompt.txt as a string to the variable beginning_chars.
  programe:-
      
      
      f = open('school_prompt.txt', 'r')
beginning_chars = f.read(30)
print(beginning_chars)



5>Challenge: Using the file school_prompt.txt, assign the third word of every line to a list called three

programe:
    
    
   three = []

with open('school_prompt.txt', 'r') as f:
    three = [line.split()[2] for line in f]
    print(three)
    
    
    
    6>Challenge: Create a list called emotions that contains the first word of every line in emotion_words.txt.
    program:-
    
      fileref = open ("emotion_words.txt","r")
line = fileref.readlines()
emotions = []
for words in line:
    word = words.split()
    emotions.append(word[0])
print (emotions)


7>Assign the first 33 characters from the textfile, travel_plans.txt to the variable first_chars.

programe:-
  f = open('travel_plans.txt', 'r')
first_chars = f.read(33)
print(first_chars)

8>Challenge: Using the file school_prompt.txt, if the character ‘p’ is in a word, then add the word to a list called p_words.

programe:-
   fileref = open('school_prompt.txt', 'r')
words = fileref.read().split()
p_words = [word for word in words if 'p' in word]


    
    
