Configure An SSH Server on your Ubuntu machine using SSHD
-----------

1. Change Listen Address on SSH config file

  - Switch into root user mode
  
  `sudo su`
  
  - Change into /etc/ssh directory
  
  `cd /etc/ssh`
  
  - Modify sshd_config file
  
  `nano ssh_config`
  
  - Change the listen address line to your IP address
  
  `ListenAddress x.x.x.x`
  
  - SAVE THE CONFIG FILE

2. Restart SSH

  - Using systemctl, restart SSH
  
  `systemctl restart ssh`
  
  - Check SSH status using systemctl
  
  `systemctl status ssh`
