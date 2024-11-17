# This is SSH configuration must likely you would use in real production environment to remotely connect to the ssh-server.
## SSH client(Windows 11):
1.Enter the command:
```
ssh-keygen
```
2. You will see option to setup password for key used for logging in using key.
3. You will generate two keys one named:
- id_rsa (Private Key which should not be shared)
- id_rsa.pub (Public Key which should be setup on server)
4. Check the public key:
  -type id_rsa.pub
5. Copy the public key and move to the server.
6. (Last Step) After the keys are setup you can use the following command to directly ssh to the server without needing to enter password:
  ```
  ssh username@ip-address-of-server
```
## SSH Server:

6.Change the directory:
```
cd .ssh
ls
```
7. Edit the authorized_keys file.
8. using nano to edit authorized_keys file:
```
nano authorized_keys
```
9. Paste the copied public key in this file.
10. Use this key combination Ctrl+s and then Ctrl+x
