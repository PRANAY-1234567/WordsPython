📘 Python Program: Count Number of Words in a Sentence

📌 Overview

This Python program counts the number of words in a given sentence entered by the user.

It uses Python’s built-in string methods to split the sentence into words and then counts them.

⚙️ Source Code
sentence = input("Enter sentence: ")

words = sentence.split()

print("Number of words:", len(words))
🧠 How It Works
1️⃣ Take Input from User
sentence = input("Enter sentence: ")
The user enters a full sentence.
Example:
Hello this is Python
2️⃣ Split Sentence into Words
words = sentence.split()
split() breaks the sentence into a list of words.
It uses space as the default separator.

Example:

["Hello", "this", "is", "Python"]
3️⃣ Count Words
len(words)
len() returns the number of elements in the list.
Each element = one word
4️⃣ Print Result
print("Number of words:", len(words))
▶️ Example Execution
Input
Enter sentence: I love programming
Output
Number of words: 3
🔑 Key Concepts Used
User input (input())
String methods (split())
Lists
Length function (len())
⏱️ Time Complexity

O(n)

The program processes each word once
⚠️ Notes

Multiple spaces are handled automatically:

"Hello   world" → ["Hello", "world"]
Punctuation (like commas, periods) will be counted as part of words.
🚀 Possible Improvements
Remove punctuation
import string

sentence = input("Enter sentence: ")
sentence = sentence.translate(str.maketrans('', '', string.punctuation))

words = sentence.split()
print("Number of words:", len(words))

📚 Learning Outcome

After understanding this program, you will learn:
How to work with strings in Python
How to convert a sentence into a list of words
How to count elements using len()

<img width="553" height="827" alt="image" src="https://github.com/user-attachments/assets/2c06a6af-ff9b-411e-be8a-6426377e1580" />
