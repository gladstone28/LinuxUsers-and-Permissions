
Users, Groups, and Permissions in Linux
Elevating Privileges (sudo)

Good security practices suggest that administrator/root access be limited. Typical day-to-day activities such as word processing, web browsing, or listening to music should never be done using the administrator account.

However, there are times when an administrator account is required to perform specific tasks, like adding and modifying permissions and configuring system software.

The 
Linux shell has the sudo command that can temporarily elevate privileges to a user that is a member of the administrator group.

Let’s say we need to modify the owner of a file named sketches.ppt from bob to debbie. We could enter the chown command with the right parameters in the terminal:

```
chown debbie sketches.ppt

```

However, if we have admin privileges but are not logged in as the administrator, this command will return an “operation not permitted” error since we don’t have sufficient privileges. But, we can use the handy command sudo in front of the same command to temporarily invoke admin privileges by confirming our identity. We can use the following command:

```
sudo chown debbie sketches.ppt

```

link to lesson:

https://www.codecademy.com/courses/introduction-to-linux-users-and-permissions/lessons/users-groups-and-permissions/exercises/elevating-privileges-sudo
