#0x12. Web stack debugging #2
+ Devops
+ SysAdmin
+ Scripting
+ Debugging
<img src="https://s3.amazonaws.com/intranet-projects-files/holbertonschool-sysadmin_devops/287/99littlebugsinthecode-holberton.jpg"/>


##Tasks
[0. Run software as another user](0-iamsomeoneelse)
<img src="https://s3.amazonaws.com/alx-intranet.hbtn.io/uploads/medias/2020/9/eaeff07a715ff880b1ceb8e863a1d141a74a7f85.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIARDDGGGOUSBVO6H7D%2F20240212%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20240212T222955Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=ecc7aa9411dd8a96d1d0cd6dfdeefcc329577aec9baf9e18828928b72d4eb5b8"/>

The user root is, on Linux, the “superuser”. It can do anything it wants, that’s a good and bad thing. A good practice is that one should never be logged in the root user, as if you fat finger a command and for example run rm -rf /, there is no comeback. That’s why it is preferable to run as a privileged user, meaning that the user also has the ability to perform tasks that the root user can do, just need to use a specific command that you need to discover.

For the containers that you are given in this project as well as the checker, everything is run under the root user, which has the ability to run anything as another user.

Requirements:
+ write a Bash script that accepts one argument
+ the script should run the whoami command under the user passed as an argument
+ make sure to try your script by passing different users

[1. Run Nginx as Nginx](1-run_nginx_as_nginx)
The root user is a superuser that can do anything on a Unix machine, the top administrator. Security wise, you must do everything that you can to prevent an attacker from logging in as root. With this in mind, it’s a good practice not to run your web servers as root (which is the default for most configurations) and instead run the process as the less privileged nginx user instead. This way, if a hacker does find a security issue that allows them to break-in to your server, the impact is limited by the permissions of the nginx user.

Fix this container so that Nginx is running as the nginx user.

Requirements:
+ nginx must be running as nginx user
+ nginx must be listening on all active IPs on port 8080
+ You cannot use apt-get remove
+ Write a Bash script that configures the container to fit the above requirements

[2. 7 lines or less](100-fix_in_7_lines_or_less)
Using what you did for task #1, make your fix short and sweet.

Requirements:
+ Your Bash script must be 7 lines long or less
+ There must be a new line at the end of the file
+ You respect Bash script requirements
+ You cannot use ;
+ You cannot use &&
+ You cannot use wget
+ You cannot execute your previous answer file (Do not include the name of the previous script in this one)

