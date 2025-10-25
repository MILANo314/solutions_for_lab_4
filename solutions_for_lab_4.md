# Exercise 1: Go to your home folder and see all files with permissions
cd ~           # go to home folder
ls -la         # list all files and folders, including hidden ones, with details (permissions, owner, size, date)

# Exercise 2: Show /var/log folder contents sorted by size, human readable, ascending
ls -lhS /var/log | tac  
# ls -l : long format, -h : human readable, -S : sort by size
# tac : reverse order to get ascending size

# Exercise 3: Create a file firstname.txt and write your first name using nano
nano firstname.txt  
# type your first name inside nano editor
# save with Ctrl+O, exit with Ctrl+X

# Exercise 4: Write your last name to lastname.txt using echo
echo "Serttas" > lastname.txt  
# '>' writes output to a file (creates or overwrites file)

# Exercise 5: Show contents of both files
cat firstname.txt lastname.txt  
# cat shows content of files

# Exercise 6: Add lastname.txt content to firstname.txt
cat lastname.txt >> firstname.txt  
# '>>' adds content to the end of the file (does not erase existing content)

# Exercise 7: Save list of folders from home to a file
ls -d ~/*/ > folder_list.txt  
# -d only shows directories
# '>' saves the list to folder_list.txt
