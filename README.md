# Linux-cheat-sheet

### Table of Contents

---

| No. | Topic                                                                   |
| --- | ----------------------------------------------------------------------- |
| 1   | [**User information**](#user-information)                               |

### User Information

1. **id:** 
It display the user identification(the real and effective user and group IDs) information

    ![id_screenshot](https://github.com/khirwadkarshubham25/ubuntu_commands/assets/122966558/11511a7b-901a-422f-ba05-7d10be0cd0f0)


2. **who** 
It is used to get information about currently logged in user on to system. If you don't provide any option or arguments, the command displays the following information for each logged-in user.

    1. Login name of the user
    2. User terminal
    3. Date & Time of login
    4. Remote host name of the user
    
    
    ![who_screenshot](https://github.com/khirwadkarshubham25/ubuntu_commands/assets/122966558/c81ce2d3-6de6-4433-a06d-5837d109979f)    

3. **whoami** 
It display the system’s username

    ![Screenshot from 2023-06-01 20-35-49](https://github.com/khirwadkarshubham25/ubuntu_commands/assets/122966558/5413fb7b-99e6-4559-8991-5821dbeec32d)    

4. **users** 
It displays usernames of all users currently logged on the system.
    
    ![Screenshot from 2023-06-01 20-37-30](https://github.com/khirwadkarshubham25/ubuntu_commands/assets/122966558/b91d038d-cb4e-47ea-bd9b-4b4a7614694f)

5. **finger**
It is used to check the information of any currently logged in users. i.e, It displays users login time, tty (name), idle time, home directory, shell name etc.
    
    ![Screenshot from 2023-06-01 20-44-07](https://github.com/khirwadkarshubham25/ubuntu_commands/assets/122966558/35cfd1a4-01ed-41ed-b9f1-0f5089ba2a20)
  
    This may not be available by default in many linux machines. In this case, you need to install it manually.

    ```bash
    $ sudo apt install finger

6. **last or lastb** 
It displays a list of last logged in users on the system. You can pass user names to display their login and hostname details.

    Syntax
    ```bash
    $ last [options] [username...] [tty...]
    ```
    
    ![Screenshot from 2023-06-01 20-51-45](https://github.com/khirwadkarshubham25/ubuntu_commands/assets/122966558/020803eb-a03e-4017-8779-ccd53a6a4e3a)

7. **lastlog:** 
This command is used to find the details of a recent login of all users or of a given user.

    ![Screenshot from 2023-06-01 20-55-46](https://github.com/khirwadkarshubham25/ubuntu_commands/assets/122966558/670b7bd5-26d0-4cf3-b11e-1391067c1f1b)

8. **W** 
It is a command-line utility that displays information about currently logged in users and what each user is doing.

    Syntax
    ```bash
    $  w [options] user [...]
    ```
    
    ![Screenshot from 2023-06-01 20-58-21](https://github.com/khirwadkarshubham25/ubuntu_commands/assets/122966558/3cb496c1-61a3-4118-adce-3682fb57056e)

9. **groups:** 
This command is used to display all the groups for which the user belongs to.

    ![Screenshot from 2023-06-01 20-59-47](https://github.com/khirwadkarshubham25/ubuntu_commands/assets/122966558/9a0c64be-c18b-41bd-a018-9ffcb03e98c8)

10. **su** 
It used to become substitute user during a login session.

    ```bash
    $ su

11. **sudo**
This command lets us use our account and password to execute system commands with root privileges.

    ```bash
    $ sudo

12. **adduser or useradd**
This command is used to creates a new user or group.

    ```bash
    $ adduser xyz
    
    Adding user 'xyz' ...
    Adding new group 'xyz' (1001) ...
    Adding new user 'xyz' (1001) with group `xyz'
    .
    .
    .

13. **userdel**
This command is used to delete the user account identified by the login parameter.

    ```bash
    $ userdel xyz
    ```
    
    userdel: user 'xyz' removed
14. **usermod**
This modifies the system account files to reflect the changes that are specified on the command line.
The below command is used to modify the user xyz. The command sets the user's real name to "xyz abc" using the -c option and changes the user's default shell to /bin/bash using the -s option.

    ```bash
    $ usermod -c "xyz abc" -s /bin/bash xyz
    ```     
    

  **[⬆ Back to Top](#table-of-contents)**
