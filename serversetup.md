```ssh root@<ip>```
```adduser <username>```
```usermod -aG sudo <username>```
exit
```
відключення входу по паролю
```ssh-copy-id -i ~/.ssh/id_rsa.pub <username>@<ip>
ssh <username>@<ip>
sudo nano /etc/ssh/sshd_config` (PasswordAuthentication no, ChallengeResponseAuthentication no, UsePAM no, PermitRootLogin no)
sudo service ssh restart >> вийти з серверу
>> перевірка **ssh root@<ip>**,  ssh <user>@<ip> -o PubkeyAuthentication=no >> Permission denied (publickey).```

sudo apt update
sudo apt upgrade -y

`sudo apt install ufw htop ccze` (встановлюємо корисні утіліти, якщо не встановлені)
`sudo ufw allow 22`
`sudo ufw enable`
`sudo ufw status`  статус
