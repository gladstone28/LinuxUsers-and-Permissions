

Users, Groups, and Permissions in Linux
Users and Groups in Linux
6 min
Now that we’ve covered how different 
Linux
Preview: Docs Loading link description
 users can coexist, let’s learn about users, groups, and their IDs!

On a Linux system, all users added are assigned a name, unique user identification (UID), group, and group identification (GID). When a user is initially created, a new UID and matching GID are assigned.

UID and matching GID numbers are assigned based on the type of user:

Administrator (root): UID and GID = 0
System user (computer-generated): UID and GID assigned from 1 to 999
Normal users (real people): UID and GID = 1000 or greater, incremented with every new user
The new user is by default assigned a matching group name (and typically a matching GID) so that the user will be a member of their own group. For example, a user stephen (UID = 1000) will also be assigned to the group stephen (GID = 1000).

We can create groups and add users to them. For example, in our diagram, we have a group called Business that includes the user Tony. Users can also exist in more than one group as well.

We can use the id and groups commands in the terminal to check our uid and gid.
