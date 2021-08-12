README
Name: Karina Sanchez
CSE135

ipv4 address to my server: 147.182.242.172
private ip: 10.124.0.2

login information for grader on Apache:
ssh key: grader@147.182.242.172
passphrase for ssh key: turtles4444
sudo password: cse135

Link to my site: https://kcs4.dev

Username for site: grader
password: turtles4444

Summary of changes to HTML file in DevTools after compression: After enabling compression the content-length of my HTML file got significantly smaller. Before, the original size of my file was 1.5KB. After compression the size is now 717B.



Summary of removing 'server' header:
First, I installed and enabled modSecurity. Then I went to the apache2 configuration file and inserted this chunk of code at the end of the file.

<IfModule mod_security2.c>
SecServerSignature "CSE135 Server"
</IfModule>

After that I restarted apache and the server header was changed to CSE135 Server.
