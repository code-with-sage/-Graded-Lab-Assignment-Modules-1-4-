1. echo "this is sample data in this file" > sample_data.txt <br>
    echo command will generate/print the given text and > will store it in newly created file sample_data.txt

2. ln sample_data.txt sample_hard.txt <br>
    ln  command will create a hardlink named sample_hard.txt to sample_data.txt 

3. ln -s sample_data.txt sample_soft.txt <br>
    when we use ln command with option -s it create a softlink here we are createing a softlink named sample_soft.txt to the sample_data.txt file 

4. ls -i sample_data.txt <br>
   ls -i sample_hard.txt <br>
   ls -i sample_soft.txt <br>
     ls command with -i option priont inode numnber of given files this command will display inode number of these files 

5. the inode number of original file (sample_data.txt) and hard link (sample_hard.txt) is same because they are pointing to the same memory location but the i node number of symbolic link(sample_soft.txt) is different because it is pointing towad the sample_data.txt file insted of its memory location. 
              if we will delete sample_data.txt we can access the file content by using hardlink sample_hard.txt but after deletation of original file sample_soft.txt will be inactive.

6. ls -l sample_data.txt <br>
   stat sample_data.txt <br>
     these both command will Display detailed file information (permissions, ownership, size, timestamps) of sample_data.txt file.

7. du -sh ~ <br>
    this command will display the disk usage of your home directory in a human-readable format.

8. ls -lh ~ <br>
     the ls command with options -l and -h will display  the size of each file present in your home directory in a human-readable format.

9. rm sample_soft.txt <br>
   ls sample_soft.txt <br>
   cat sample_data.txt <br>
      rm command will remove the sample_soft.txt named softlink then we us ls to verify it is removed lastly we use the cat command for sample_data.txt file to verify that original file is not affected 

10. du sample_data.txt <br>
      displays disk space used by the file sample_data.txt, showing how much storage that specific file occupies.

du -sh ~ shows total disk usage of the home directory in human readable format, summarizing all contained files and folders.

df displays filesystem disk space usage, showing total blocks, used space, available space, and mount points.

df -h displays filesystem disk usage in human readable units like KB, MB, and GB for easier understanding.


