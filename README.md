# basic-playbook

> This file will document my progression through the Cloud Academy 'Getting Started with Ansible' Lab but within my own local environments.<br/>
> The objective is to further push my practice into more realistic settings that may be more like the working environments that I am applying for.<br/>

## lamp.yml

> This playbook uses ansible to configure and set up an apache2 webserver on the local host.

## lamp-vars.yml
> This version of the playbook does the same thing as the original version however it impliments the use of variables within the play.<br/>
- This play also enables the apache server to enable HTTPS using shell commands via the ansible shell module <br/>
sudo asemod ssl <br/>
sudeo a2ensite default-ssl <br/>


 
## Amazon Web Services 
- Making an IAM user account with the correct permissions 
- Creating ec2 instance and updating security group to allow ssh access ( this tripped me up yesterday)
- Personally noticed that to ssh into ec2 instance from my windows machine running an ubuntu system I needed to use sudo before the command as opposed to the normal approach<br/>
(superuser.com,2018)<br/>
- After running ansible-playbook <playbookfile> command vs code always disconnects from the vm and times out upon reconnecting.

# References 
 superuser.com, 2018, Windows ssh permissions for private key are to open [Forum] Link: https://superuser.com/questions/1296024/windows-ssh-permissions-for-private-key-are-too-open visited: 20/10/22
