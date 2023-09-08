
# Linux Permissions

In Linux, permissions are often represented in octal (base-8) format rather than hexadecimal (base-16) format. Octal notation is more commonly used because it maps directly to the binary representation of permissions.

The octal representation of permissions uses three digits, where each digit represents the permissions for the owner, group, and others, respectively. Each digit is calculated by assigning values to read (4), write (2), and execute (1) permissions and then adding these values to represent the desired permissions.

Here's how the octal permissions work:

Read (r): 4

Write (w): 2

Execute (x): 1

To calculate the octal permission value, you sum up the values of the desired permissions. For example:

Read and write permission: 4 (read) + 2 (write) = 6

Read, write, and execute permission: 4 (read) + 2 (write) + 1 (execute) = 7

No permissions (none): 0

Here are some common octal permission values:

0: No permissions

1: Execute only

2: Write only

3: Write and execute

4: Read only

5: Read and execute

6: Read and write

7: Read, write, and execute

For example, if you want to set read and write permissions for the owner, read-only permissions for the group, and no permissions for others on a file, you would use the octal value 640:

Owner: Read (4) + Write (2) = 6

Group: Read (4) + No permissions (0) = 4

Others: No permissions (0)

So, chmod 640 <file> would set these permissions.


While octal notation is the standard way to represent permissions in Linux, it's worth noting that you can convert octal values to hexadecimal if you need to, but this is not a common practice for representing permissions. 
