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
###        ###
*/
blank = []
email = 'name@domain.com'
email2 = email.split('@')
email3 = email.split('.')

print(email2[1].split('.'))
print(email2)
#print(email3)


blank.append(email2[0])
blank.append(email2[1].split('.')[0])

print(blank)
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
