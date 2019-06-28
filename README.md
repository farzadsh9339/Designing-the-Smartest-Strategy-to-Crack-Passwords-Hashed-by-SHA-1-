# Designing the Smartest Strategy to Crack Passwords Hashed by SHA-1

In this project, we are given a password file “passwords.txt”, the file lists a number of passwords,
however, in SHA-1 hashed version. Each line of the file has the following format: [User ID] [SPACE]
[SHA-1 Hash of The User’s Password]. Our goal in this project is to crack the passwords in the file as many as possible. We are given
the following knowledge about the (bad!) practice of people setting up their passwords; Some people tend to use only a few digits as passwords or some people tend to use English words or phrases or short sentences as passwords or some people combine English words and numbers, but they generally place few numbers after the English words.
In this project, we assume that all English words are lower-case, and all of them are chosen from a given dictionary file “dictionary.txt” and we add another dictionary file wordlist.txt which all numbers are chosen from it. We use Python to design the password cracking system.
We wrote a python code which is attached to this report. The strategy falls into two main sections. First, using the dictionary attack and then performing brute-force attack.
When the code is run, it first asks you which attacking strategy the user wants to proceed with. Then, if the user wants to proceed with the dictionary-based attacking strategy, a dictionary is needed to be imported. In the first attack strategy which is using the dictionary, initially we wrote a code which loads and imports the given dictionary in python. Then, the code asks you about the hash. By the given hash it tries to crack it and find the original word which is nothing but trying to calculate SHA1 hashes of all given words in the dictionary and compare them with the given hash.
As mentioned before, the dictionary contains only lower-case words without any numbers, and the hashed passwords represent words or numbers or the combination of words and numbers.
