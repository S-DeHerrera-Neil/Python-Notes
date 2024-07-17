# Day_1 07/15/2024 

# '''(Tripple quote for Multi-Line comments)

        
This command will login to our linops as student:
# 10.50.27.61(linux/lin-ops) 10.50.39.134(Windows/)
# command: terminator (opens a terminal that allows you to split screens)
## SSH Command ##
'ssh student@10.50.27.61 -X'
        ## For Loop ##
 This is a for loop example
"Print each fruit in a fruit list:"

fruits = ["apple", "banana", "cherry"]
for x in fruits:
print(x)


# Day_2 07/16/2024 
        # *Activity - Split an email Address
email = 'name@domain.com'

## Email Activity ##

email = "name@domain.com"

EmailUserName = email.split('@')
EmailDomain = '.'.join(EmailUserName)
EmailTLD = EmailDomain.split('.')

print(EmailTLD)

#list = ['name', '@domain', 'com']
#Desired Result^


##Fellowship Example .append()##

#!/usr/bin/env python3

fellowship = []
fellowship.append('Frodo')
fellowship.append('Sam')
fellowship.append('Mary')
fellowship.append('Pip')
print(fellowship)


### Spliting and Appending Email Addresses ###

blank = []
email = 'name@domain.com'
email2 = email.split('@')

blank.append(email2[0])
blank.append(email2[1].split('.')[0])
blank.append(email2[1].split('.')[1])

print(blank)

## Flow Controls input() ##
        #Bad Eaxmple Below#
        '''
        input ('Type Something :\n')
        num = int(input('Type a number:\n'))
        if num == 7:
    print('This is True')
        elif num > 7:
        print('num ' + str(num) + ' is < 7')
        elif num > 7 and num < 20:
        print(str(num) + ' is between 7 and 20')
        else: 
        print('This is the end, thank goodness')
        '''

## FizzBuzz example ## I did this one!!!

num = int(input('Guess a number:\n'))
if num %3 == 0 and num %5 == 0:
    print('fizzbuzz')
elif num %5 == 0:
    print('buzz')
elif num %3 == 0:
    print('fizz')
else:
        print('This is the end, thank goodness')
# on vim make sure you have the appropriate indentations & print(num)


## For Loop example 1 ##

beer = ['Coors', 'Coors Light', 'Coors Banquet']
for anything in beer:
    print(anything)

## For Loop example 2 ##

xmen = ['Superman', 'Night Crawler', 'Deadpool', 'Storm']
for hero in xmen:
    if hero == 'Superman':
        print('WRONG UNIVERSE')
    elif hero == 'Deadpool':
        print(hero + 'is the best one!')
    else:
        print('This is a Marvel hero')


## While loop example 1 ##

#while <condition>
num = 0
while num < 5:
    print(num)
    num += 1
        ## Pass, Break, Continue and Return Examples ##

def test():
    while True:
        usr = input("Type 'Pass', 'Break', 'Continue' or 'Return':\n ").lower()
        if usr == 'pass':
            pass
            print("This is 'pass'. ")
        elif usr == 'break':
            break
            print("This is 'break'")
        elif usr == 'continue':
            continue
            print("This is 'continualphabet = []
                for i in range(97,123):
     alphabet.append(chr(i))
 ###
alphabet
['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z']
>>> 
e'")
        elif usr == 'return':
            return "This is 'return'"
        else:
            print('Please choose a valid option.')
        
test()
        
#'HeLlo'.upper
#'HeLlo'.lower
        
        # Practical Exercise 0-1 - Configure your editor
        # Activity - Split an email address
        # Practical Exercise 0-2 - FizzBuzz
# Day_1 07/17/2024 
        
        # Practical Exercise 0-3 - Guess the Number

#!/usr/bin/env python3

def guess_number(n):
    while True:
        usr = int(input('Guess a Number between 0-100:\n'))
        if n == usr:
            print('WIN')
            break
        elif usr < n:
            print('too low')
        elif usr > n:
            print('too high')
guess_number(23)

## make a list called alphabet
alphabet = []
for i in range(97,123):
    alphabet.append(chr(i))
 
alphabet
#Result is lower case alphabet put in list called alphabet
['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z']

## Game example ##
inventory = {'CFB25': 69.99, 'MVP': 149.99, 'wheels': 5}
 for game in inventory:
     print(inventory[game])
##
order = (['wheels',5],['MVP' ,2])
order
(['wheels', 5], ['MVP', 2])
inventory = {'CFB25': 69.99, 'MVP': 149.99, 'wheels': 5}
order
(['wheels', 5], ['MVP', 2])
for i in order:
     print(i)
           

['wheels', 5]
['MVP', 2]
 order
(['wheels', 5], ['MVP', 2])
 order[0]
['wheels', 5]
 order[0][-1]
5
 for i in order:
     total += inventory[i[0]] * i[1]
     print(total)

## How SSgt Rung wants us to open files ##
with open("test.txt") as fp:
    pass
##
fp.write('First line\n')
     lines = ['Second line\n', 'Third line\n', 'Fourth line\n', 'Last line\n']
     fp.writelines(lines)

#runestone examples#

#1 The textfile, travel_plans.txt, contains the summer travel plans for someone with some commentary. Find the total number of characters in the file and save to the variable num.
with open('travel_plans.txt') as fp:
    num = len(fp.read())
print(num)

#2 We have provided a file called emotion_words.txt that contains lines of words that describe emotions. Find the total number of words in the file and assign this value to the variable num_words.
with open('emotion_words.txt') as fp:
    num_words = len(fp.read().split())

#3 Assign to the variable num_lines the number of lines in the file school_prompt.txt.
with open('school_prompt.txt') as fp:
    num_lines = len(fp.readlines())

#4 Assign the first 30 characters of school_prompt.txt as a string to the variable beginning_chars.
with open('school_prompt.txt') as fp:
    beginning_chars = fp.read(30)
    print(beginning_chars)

#5 Challenge: Using the file school_prompt.txt, assign the third word of every line to a list called three.
three = []
with open('school_prompt.txt') as fp:
    for line in fp:
        three.append(line.split()[2])

#6 Challenge: Create a list called emotions that contains the first word of every line in emotion_words.txt.
emotions = []
with open('emotion_words.txt') as fp:
    for line in fp:
        emotions.append(line.split()[0])

#7 Assign the first 33 characters from the textfile, travel_plans.txt to the variable first_chars.
with open('travel_plans.txt') as fp:
    first_chars = fp.read(33)

#8 Challenge: Using the file school_prompt.txt, if the character ‘p’ is in a word, then add the word to a list called p_words.
p_words = []
with open('school_prompt.txt') as fp:
    for line in fp:
        for word in line.split():
            for char in word:
                if char == 'p':
                    p_words.append(word)
                    break


# Practical Exercise 1-1 - Invert and Inverted
# Practical Exercise 1-2 - Least Significant Bit (LSB) Steganography - Encode a Single Character
# Practical Exercise 1-3 - Least Significant Bit (LSB) Steganography - Encode Multiple Characters
# Practical Exercise 1-4 - Portable Grey Map Steganography
# Practical Exercise 2-1 - Raw Portable Grey Map LSB Steganography
# Practical Exercise 2-3 - Botnets
