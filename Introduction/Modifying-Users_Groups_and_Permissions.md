
# Users, Groups, and Permissions in Linux

#### Modifying Users, Groups, and Permissions


Linux provides users the ability to elevate or relax access permissions on any files where they are an owner. Of course, an administrator can make changes anywhere in the system, including creating users and groups, modifying them, and elevating or reducing any permissions for files.


#### Adding and Modifying Users and Groups

As an administrator, there are commands at your disposal to add, delete, or modify users and groups:

- useradd creates a new user
- groupadd creates a new group
- usermod and groupmod can be used to modify users and groups
- userdel and groupdel can be used to delete users and groups.


#### Modifying Owners and Permissions

Additionally, chown and chgrp allow the superuser/admin to change who owns the resource, file, or directory while chmod changes the read-write-execute permission levels. As an example, the following commands would allow an administrator to change the owner of a file named designs.doc to a new user named peter and then modify this file to have read, write, and execute permissions for the user, group, and others.


```
chown peter designs.doc

```
also

```
chmod 777 designs.doc
or
chmod u=rwx,g=rwx,o=rwx designs.doc

```
Note: We need to be the owner of the file or admin to use chmod.

#### Viewing and Modifying Permissions Outside of the Terminal

We can view and modify permissions in the file manager application on a Linux Ubuntu desktop as well. Just right-click on the file, select properties from the drop-down, and choose the permissions tab. All the users/groups and permissions are easily selected from the drop-down menus.


![](./ gui_permissions.png)
