|Command|Description|
|---|---|
|`useradd -G [group_name] [username]` or `useradd [username]`|Add new user|
|`userdel [username]`|Delete user|
|`groupadd [group_name]`|Create new group|
|`usermod -a -G [group_name] [username]`|Add existing user to a group|
|`passwd [username]`|Change password|
|`groups` or `cut -d: -f1 /etc/group`|List all linux groups|
|`groups [username]`|List user groups|
