# VBox_Docker_N8n

# 1) Download Ubuntu 22.04 Desktop Image from https://releases.ubuntu.com/jammy/

<img width="1417" height="795" alt="image" src="https://github.com/user-attachments/assets/4c16d2a5-322f-4783-939f-2e9439e4e126" />

# 2) In Virtualbox, add a new virtual machine and use the image that you downloaded.

<img width="553" height="377" alt="image" src="https://github.com/user-attachments/assets/014d795f-a974-49c2-bc54-e0c78f4bdfe9" />

Under Unattended Install change the username and password to something you will remember. 

<img width="427" height="283" alt="image" src="https://github.com/user-attachments/assets/7b6cc123-43b6-48b9-9259-7292e142c6c5" />

Under Hardware, change memory to at least 4096 MB and processors to at least 2.

<img width="912" height="436" alt="image" src="https://github.com/user-attachments/assets/f8e563d9-b9eb-4032-b545-2b8dfee845d9" />

# 3) After the first startup, shut down the instance and go to Settings and click Advanced under General. In the Shared Clipboard, select Bidirectional.

<img width="287" height="41" alt="image" src="https://github.com/user-attachments/assets/b244a848-48f0-4aa6-a0e0-db040d196d12" />

Scroll down to Network and for Adapter 1, select NAT. Then for Adapter 2, select Host-only Adapter and switch Promiscuous mode to Allow VMs. 

<img width="651" height="347" alt="image" src="https://github.com/user-attachments/assets/2a32550b-7817-4cfb-a256-98b7955837d7" />

When running sudo update && upgrade, you may need to add your user account to the sudoers file. To solve this, type "su -" to login as the root user and use the same password that you are using for your user account. Then run "sudo adduser [username] sudo" and restart the machine.

verify that your user is in the vboxsf group by running sudo adduser $USER vboxsf
<img width="547" height="152" alt="image" src="https://github.com/user-attachments/assets/02d917a3-98f5-4e59-bd30-005b23a87a68" />

then change shared clipboard and drag and drop to bidirectional.
then use sudo reboot to restart the instance

<img width="786" height="557" alt="image" src="https://github.com/user-attachments/assets/88834ddd-070d-459e-be22-0974d703c3a6" />


https://dockhand.pro/

<img width="767" height="595" alt="image" src="https://github.com/user-attachments/assets/b2cd4a90-7809-45cb-aa64-1c772dd1c71f" />
