# There is ssh-server and a ssh client to perform remote operation on ssh-server.(entire setup is in on same netwok)
## SSH-Server is Ubuntu system in this Scenerio.
1. We need to setup these things:
```
sudo apt install openssh-server
sudo systemctl enable ssh
sudo systemctl start ssh
sudo systemctl status ssh
```
2. Next step, to allow ssh in firewall as ubuntu use "UFW firewall":
```
sudo ufw allow ssh
sudo ufw enable
sudo ufw staus

```
3. Copy the ssh-server IP address after running the command below:
```
ip a
```

## SSH-Client is Windows system in this Scenerio(Using Windows 11).
```
ssh username@ip-address-of-server
```
4. type yes
5. Enter Your server user password
### Wollah you are login i think
