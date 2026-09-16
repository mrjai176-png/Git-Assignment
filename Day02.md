*Git Reset:
It is used to uncommits the sequential commits from local repo
    # Soft reset :
          It uncommits the commit from local repo to working directory and changes made in that commit is sent to working directory. Just copy and paste the previous commit id of the file so that the commits after the given commits will be reseted
           git reset <commit id of previous file>
    # Hard reset :
          It removes the file from the directory and also uncommit the commit .Just copy and paste the previous commit id of the file so that the commits after the given commits will be reseted
           git reset --hard <commit id of previous file> 

         *Soft reset eg
           Local repo commits 
           file1
           file2
           file3
           file4
           file5

          In soft reset if you want to uncommit from file3 - file5 just paste the commit id of the file2

          result
          Local repo         working directory (files untracked)
          file1                file3,file4
          file2                  file5
          
        *Hard reset
         Local repo commits
         file1
         file2
         file3
         file4
         file5

        In hard reset the files from the local repo is uncommited and removed from directory

        result
        local repo       working dir
        file1           no files as the other 3 files are removed and other 2 in local repo
        file2
