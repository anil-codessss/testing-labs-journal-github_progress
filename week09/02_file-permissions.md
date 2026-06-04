# Understanding File Permissions

## Task 1 --- Create a File

Run:

    touch secret.txt
    ls -l secret.txt

### Screenshot

(Add screenshot here)

### Questions

1.  Who owns the file?
   ans: The file is owned by the user who created it such as pi.
3.  What are the default permissions?
   ans: The default permissions are read and write.
### Reflection

Why is file ownership important in Linux systems?
Ans: The file ownership is important because it determines who can access, modify,or delete a file. It helps protect data from unauthorized user and ensure that only the appropriate user or process can make changes, improving system security and privacy.
------------------------------------------------------------------------

## Task 2 --- Restrict File Permissions

Run:

    chmod 600 secret.txt
    ls -l secret.txt

### Screenshot

(Add screenshot here)

### Questions

1.  Who can read the file now?
    Ans:The owner can read the file now.
3.  Who cannot access it?
    Ans:The members of the group and all other user can not read, write or execute the file.

------------------------------------------------------------------------

## Task 3 --- Open Permissions (Security Risk)

Run:

    chmod 777 secret.txt
    ls -l secret.txt

### Screenshot

(Add screenshot here)

### Questions

1.  Who can access the file now?
    Ans:The owner, group members and all other user acess the file.
3.  Why might this configuration be dangerous?
    Ans : This configuration is dangerous because any user on the file contents,insert malicious code,or delete important data. For sensitive files, permission such as 600 or 640 are much safer than 777.
