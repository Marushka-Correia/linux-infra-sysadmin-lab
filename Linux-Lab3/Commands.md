# 1️) Check current user
whoami


# 2️) Create a new user
- sudo adduser testuser

I was asked to :
Set a password
Press ENTER for other details
output:  User created

# 3️) Verify the user exists
- id testuser


# 4️) Create a group
- sudo groupadd devops

Output: Group created

# 5) Check the group
- getent group devops


the output i obtained: devops:x:1002:

# 6) I tried adding the created user to the group I previously created
- sudo usermod -aG devops testuser

 Things which are necessary to remember:
# -a means append

# Without -a, user can lose other groups


# 7️) Verify user group membership
groups testuser

The output I obtained:
testuser : testuser devops
which means that user was added to group

# 8️) log in as the new user
su - testuser
I was asked to enter the password I set initially

# 9) How to check user
- whoami
Output:testuser
