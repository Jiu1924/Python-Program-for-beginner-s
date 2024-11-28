# Python-Program-for-beginner-s
# Program 1: Write a Python Program Program to count the occurrence of each word in a given sentence.

#Define a Function
def word_count(sentence):
     
     #.lower() Convert the whole sentence in lower case to avoid case-insensitive 
    sentence = sentence.lower()
    unique_words = "" #Initialize empty string

    #looping
    for word in sentence.split():

        if word not in unique_words:
            print(f"{word}: {sentence.count(word)}")

            #It add the current word to the unique_words string and Ensures that each word is only counted once.
            unique_words += word +" "

word_count(input("Enter Your sentence : "))

#Program 2 Write a Python Program to remove  a newline in Python

#Input the Sentence
text = "\nBest \nDeeptech \nPython \nTraining\n"

result = ""#Initialize empty string

#looping
for char in text:
    if char != "\n":
        result += char
print(result) 


#Alternative method to remove newline by .replace function
string = "\nBest \nDeeptech \nPython \nTraining\n"
result = string.replace("\n", "")
print(result)

# Program 3 : Write a Python program to reverse words in a string

#Define a function
def reverse_words(text):
    words = text.split()
    reversed_words = words[::-1]
    return ' '.join(reversed_words)

#Input a Sentence or Word
text = input("Enter your Sentence or words :")
print(reverse_words(text))  


#Program 4: Write a python program to count and display the vowels of a given text

#Input the sentence
text = input("Enter your Sentence: ")
vowels = 'aeiouAEIOU'
count = 0

#looping
for char in text:
    if char in vowels:
        count += 1
        print(f"Vowel found: {char}")

print(f"Total vowels: {count}")

