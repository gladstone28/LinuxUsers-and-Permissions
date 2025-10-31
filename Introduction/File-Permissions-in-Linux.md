
Users, Groups, and Permissions in Linux
File Permissions in Linux

How do users and groups relate to what files they can access?

If we use the command ls -l on a working directory, we will see directory/file permissions, user, group, filesize, creation date/time, and filename.

In 
Linux, everything is based on file permissions. Each file or directory has an owner and a group (or groups) that usually has more permissions to read, write, or execute than users not in the owner or in the permission group.

```


```
Let’s break down the permissions line for file-1.txt from the screenshot:

```
-rw-rw-r--

```
Note: the first character identifies the resource as either a directory (d) or file (-).

The following nine characters should actually be read as triplets: rw- for the file owner, rw- for the group(s) that have permission to the file, and r-- for all others. What do these symbols mean?

- read (r) = contents can be viewed but not edited, renamed, added, or deleted
- write (w) = contents can be viewed, edited, renamed, added, and deleted
- execute (x) = contents can run as a program or script
- (-) = permissions don’t apply

So, the permissions shown for file-1.txt means that the owner can read and write, the group can read and write, and all others can only read.

Read-write-execute permissions can also be written as numbers, with each being a power of two. Each set of triplets can be expressed as the sum of the permissions that apply.

```

```

For example, a file’s permission being 777 is equivalent to rwxrwxrwx, whereas a file’s permission being 755 is equivalent to rwxr-xr-x.


Default Permissions
When a normal user creates a folder, the default owner for the user and group is set to the username. The default permissions are typically set to 755 (or “rwx” for the user, “rx” for the group, and “rx” for others). These defaults are designed to restrict access until deliberately granted!

When a user then creates a file inside the folder, the default owner for the user and group is again set to the username while the permissions for that file are set to 644 (or “rw” for the user, “r” for the group, and “r” for others).

In the following exercise, we’ll go over how these permissions can be changed!


#### Exercise


