# The Linux Command Line Lab

## Task 1: Changing to the Root User

**Commands / Description:**
sudo su root / This command allows a user to run with superuser permissions to become the root user. 

**Screenshot:**
![Task 1](../images/task1.png)

## Task 2: Creating User with Useradd and Adduser

**Commands / Description:**
sudo useradd bobby, sudo adduser sally / The difference between these two commands is that when you're using the command "adduser" it's a more informative and secure approach. After "useradd" it didn't mention anything else as opposed to "adduser" which told me it was being added as a user, a group, given a home directory, and asked me to type a password as well.

## Task 3: Switching the User

**Commands / Description:**
sudo su - sally / This command prompts me to enter my password which results the main user to be changed to sally, a user that was created using "adduser" command.

**Screenshot:**
![Task 3](../images/task3.png)

## Task 4: Adding Users after Switching Users

**Commands / Description:**
sudo useradd earl / After running this command the prompt tells me "sally is not in the sudoers file. This incident will be reported". The reason this occurs because sally is a normal user and doesn't have root privileges so it doesn't allow her to perform such action.

## Task 5: Peforming Tasks as Original User

**Commands / Description:**
exit / Despite the benefits of completing tasks and commands as the root user it's bad practice to stay logged in as root because you can make critcal mistakes much easier. Being the root user means you have power to everything just as the saying says "great power comes with great responsibility" and this can lead to files being changed or even deleted accidentally. Additionally, being the root user can leave you vulnerable to attackers which could lead them to have entire control of your system.

## Task 6: Deleting Users and Viewing your User ID

**Commands / Description:**
sudo userdel earl, id -u 
