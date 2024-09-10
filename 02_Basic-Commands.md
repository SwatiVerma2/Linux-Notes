# Basic Commands

### 1. How to check Hostname on Linux - using `hostname`

    $ - normal user

    #- root or admin user

    Hostname - to uniquely identify the device over network

### 2. How to check current login user : 
   -  `whoami`
   
  ![image](https://github.com/user-attachments/assets/79aa3c69-9125-421f-aa77-125d556ad064)

### 3. How to check IP on Linux

 - IP address is a unique address that identifies a device on the internet or a local network.

  ![image](https://github.com/user-attachments/assets/1b7d3d97-0b6e-4ca4-a945-0602fc10910d)

### 4.Print Working Directory:
- `pwd`

  ![image](https://github.com/user-attachments/assets/aed09d90-f60e-40f9-87dc-de19e127c262)

### 5.List directory command: `ls`

   ![image](https://github.com/user-attachments/assets/92607e6f-6203-4816-9dd6-87b2ecfc7251)

  - Permissions and ownership of files explained
      ![image](https://github.com/user-attachments/assets/bbc623a7-82c1-4aa3-ade6-7910fb74d9ef)
  - Execute - deletion, modification

### 6. How to make folder on linux using mkdir
   
- You can also create directories with multiple levels (subdirectories) using the -p option, which allows you to create parent directories if they do not exist. 

 `mkdir -p parent_directory/child_directory`

 ![image](https://github.com/user-attachments/assets/32f86752-cac2-4b82-99cd-96819448466c)

- In this example, the mkdir command will create both the "parent_directory" and the "child_directory" if they don't already exist.

### 7. How to change location or move to other folder - `cd <directory-name>`

### 8. To clear the terminal: `clear`

### 9. How to create new, empty files file in linux: 

  - `touch <fine-name>`
  - Create Multiple Files: `touch file1.txt file2.txt file3.txt`
    
    ![image](https://github.com/user-attachments/assets/120f7735-401e-4fb9-8fc3-5d0b2333e931)

  - `touch file{1..10}.txt`
    
    ![image](https://github.com/user-attachments/assets/aaf5c051-c994-4329-99dc-de61335e60f0)

### 10.How to delete a folder

- `rmdir <directory-name>`
- rmdir: removing empty directories (folders). If a directory contains any files or subdirectories, rmdir will not delete it and will produce an error message.
- It is a safe way to remove directories as it won't delete the directory if it contains any content.
  
- `rm -r <directory-name>`
- The rm command, when used with the -r (or -R) option, is used to remove directories and their contents recursively. 
- This means it will delete not only the specified directory but also all the files and subdirectories within it.
- It is a more powerful and potentially dangerous command, as it can result in the loss of a lot of data if used incorrectly.

- Case 1: Removing multiple files with name starting with x : * wildcard: `rm x*` , `rm abc{1..6}.txt`
- Case 2: Delete empty directories:  `find . -type d -empty -delete`
- Case 3: Delete empty files: `find . -type f -empty -delete`
    

### 11. How to edit and write into a file 

- `vi <file-name>`
- to save and quit - :wq
- to quit without save - :q!
- vi - vi editor is a popular and powerful text editor.
- Switching Modes: vi has different modes. There are primarily two important modes: Command Mode and Insert Mode.
- Command Mode: When you open a file, you are in Command Mode. In this mode, you can navigate and perform various commands (e.g., save, quit, copy, paste, etc.). 
- Insert Mode: To start typing and editing the file, press i to enter Insert Mode. You can then type and make changes

### 12. How to login as root → su -

### 13. How to read a file

- `cat <file-name>`
- cat (concatenate): cat is a simple utility used to display the entire contents of one or more text files to the terminal. 
- It is most commonly used to quickly display the content of a file, and it's often used in combination with other commands or for redirection (e.g., sending file contents to another command or a file).
    ![image](https://github.com/user-attachments/assets/12dc3e0d-b58b-453b-8e67-efba7cabca17)

- `less <file-name>`
- less is a more feature-rich text viewer that allows you to view text files interactively.
- It is designed for navigating and reading text files, especially large ones. 
- less enables you to scroll through the file, search for text, navigate to specific lines, and more.
- It provides a more user-friendly interface for exploring text files.
- Press q to quit this
- using less command:
- Search words in your file
- Shift G - end of file
- P - start of file
- /word to be searched 
- Press n to search next instance

### 14. What is word count command

- wc: is used to count the number of lines, words, and characters (bytes) in a text file. Its name stands for "word count”.
  
    ![image](https://github.com/user-attachments/assets/657e8113-064b-4e97-b99b-b55b669226fa)

- wc -l : to check lines only
  
    ![image](https://github.com/user-attachments/assets/609468f4-5234-4f1b-ae9a-b8b64506a458)


### 15. Compare two files using diff command- compares the file line by line

`diff <file-name1> <file-name2>`

![image](https://github.com/user-attachments/assets/a10e177c-7b4f-474f-925a-dacd57ac2ed7)

