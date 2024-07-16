# Day_1 07/15/2024 

# '''(Tripple quote for Multi-Line comments)

        ## SSH Command ##
This command will login to our linops as student:
# 10.50.27.61(linux/lin-ops) 10.50.39.134(Windows/)
# command: terminator (opens a terminal that allows you to split screens)
'ssh student@10.50.27.61 -X'
        ## For Loop ##
 This is a for loop example
"Print each fruit in a fruit list:"
```
fruits = ["apple", "banana", "cherry"]
for x in fruits:
print(x)
```

# Day_2 07/16/2024 
        # *Activity - Split an email Address
email = 'name@domain.com'

## Email Activity ##
/*
email = "name@domain.com"

EmailUserName = email.split('@')
EmailDomain = '.'.join(EmailUserName)
EmailTLD = EmailDomain.split('.')

print(EmailTLD)

#list = ['name', '@domain', 'com']
#Desired Result^
*/

##Fellowship Example .append()##
/*
fellowship = []
fellowship.append('Frodo')
fellowship.append('Sam')
fellowship.append('Mary')
fellowshit.append('Pip')

*/
### Spliting and Appending Email Addresses ###
*/
blank = []
email = 'name@domain.com'
email2 = email.split('@')

blank.append(email2[0])
blank.append(email2[1].split('.')[0])
blank.append(email2[1].split('.')[1])

print(blank)
*/
## Flow Controls ##
        #Bad Eaxmple Below#
/*
input('Type Something: ')

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
*/
## FizzBuzz example ## I did this one!!!
/*
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
*/

## For Loop example 1 ##
/*
beer = ['Coors', 'Coors Light', 'Coors Banquet']
for anything in beer:
    print(anything)
*/
## For Loop example 2 ##
/*
xmen = ['Superman', 'Night Crawler', 'Deadpool', 'Storm']
for hero in xmen:
    if hero == 'Superman':
        print('WRONG UNIVERSE')
    elif hero == 'Deadpool':
        print(hero + 'is the best one!')
    else:
        print('This is a Marvel hero')
*/
        # Practical Exercise 0-1 - Configure your editor
        # Activity - Split an email address
# Practical Exercise 0-2 - FizzBuzz
# Practical Exercise 0-3 - Guess the Number
# Practical Exercise 1-1 - Invert and Inverted
# Practical Exercise 1-2 - Least Significant Bit (LSB) Steganography - Encode a Single Character
# Practical Exercise 1-3 - Least Significant Bit (LSB) Steganography - Encode Multiple Characters
# Practical Exercise 1-4 - Portable Grey Map Steganography
# Practical Exercise 2-1 - Raw Portable Grey Map LSB Steganography
# Practical Exercise 2-3 - Botnets
