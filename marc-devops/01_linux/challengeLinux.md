# Task Description:

Solve the tasks below and document your solution paths in the form of comments within the respective Bash file. It's not necessary to create a separate file for each task/script; for the simpler tasks, it's sufficient to write the solutions under the question. For the advanced tasks, however, you should create a separate file and place it in a separate solution folder, this folder is already created in the shared GitHub repository.

## Task 1: Basic Commands

# Navigate to the home directory.
# ls

# Create a new directory named "CLI-Exercise".

# mkdir CLI_Exercise

# Change to the new directory.

# cd CLI_Exercise

# Create an empty text file named "notes.txt".

# touch notes.txt

# List the contents of the directory to ensure the file was created.

# ls CLI-Exercise

# Append the text "First Note" to the file "notes.txt".

# echo "First Note" >> notes.txt

# Display the contents of the file "notes.txt".

# cat notes.txt

## Task 2: File and Directory Renaming

# Rename the file "notes.txt" to "my_notes.txt".

# mv notes.txt my_notes.txt

# Create a new directory named "Backup".

#mkdir Backup

# Move the file "my_notes.txt" to the "Backup" directory.

# mv my_notes.txt Backup

## Task 3: File Search and Filtering

# Change back to the home directory.

# cd .. | cd ..

# Create multiple text files with different names and the text content "important" using a for-loop.

# for i in a b c d e f g
# do
# echo important > $i.txt
# done

# Search for all files in the solution directory that contain the word "important".

# grep -R "important" .

# Delete all found files.

# grep -Rl "important" . |xargs rm -f

## Task 4: Pipelines and Command Combinations

# Create a text file "numbers.txt" and add some numbers (one per line).

# touch numbers.txt
# for i in 2 3 4 6 87 89
# do
# echo $i >> numbers.txt
# done

# Filter the file "numbers.txt" for lines that are greater than 50.

# awk '$1>50' numbers.txt

# Sort the filtered numbers in ascending order.

# sort numbers.txt

# Calculate the sum of all numbers in the sorted list.

# awk '{sum +=$1} END {print sum}' numbers.txt

## Task 5: Environment Variables and Command Parameters

# Create an environment variable named "MY_NAME" and set it to your name.

# export MY_NAME=ilyas

# Write a shell script named "greeting.sh" that outputs "Hello, <YOUR NAME>!",

# where <YOUR NAME> is replaced by the value of the set environment variable.

# echo -e '#!/bin/bash\necho "Hello, $MY_NAME"'>>greeting.sh
# chmod +x greeting.sh
# sh greeting.sh

# Give the script the ability to accept a greeting text

# as a parameter, and adjust the output accordingly. - also document your input.

# echo '$1' >> greeting.sh
# sh greeting.sh "how are you?"

## Task 6: Advanced Scripts (please save each as a separate file and place in a separate folder)

# Backup Script: Create a script that automatically creates backups of

# certain files or directories. You could use a

# timestamp or version number convention to name the

# backup files.

# Word Counter: Write a script that counts and outputs the number of words in a

# given file.

# Search and Replace: Develop a script that searches for a specific

# string in a file and replaces it with another string.

# Automated File Processing: Write a script that automatically

# reduces images in a directory to reduce their file size.

# Password Generator: Create a script that generates random passwords.

# You could use parameters to adjust the length and the

# use of special characters.

# Text-based Game: Create a simple text-based game

# where the player can make decisions that influence the course

# of the story - use only variables, echo, read, case, if & else commands and queries

# Tip: Decisions/probabilities can be queried via a modulo (%) function

# System Monitoring: Develop a script that displays important

# system information such as CPU usage, memory usage, and

# connected hardware.
