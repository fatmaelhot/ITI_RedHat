LAP 1
-----------------------------------------------------------
2-cat: scroll off and display the end of pages
more: display output one screen at one time (page by page) 
3-rm: to remove files
rmdir: to remove directory 
4-/home --> mkdir dir1 doc
/home/dir1 --> mkdir dir11 dir12
/home/doc --> touch mycv
/home/dir1/dir11/ --> touch file1
4-a-rmdir dir11
4-b- rmdir -p
4-c- home
./home

5-cp etc/passwod  home/mypasswod
6-mv mypasswd oldpasswd
7-../../home or cd /home   or cd ~home or cd-home 
8-ls w*
9-head -4 etc/passwod
10-rail -7 etc/passwod
11- man -a passwod
12-man passwod
13-man -K

--------------------------------------------------
Lab2
-------------

1-sudo useradd -c "islam asker" -m islam
sudo passwd islam
![photo_5987695585202912751_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/38af4ac1-ba78-4467-94aa-42bc806f0079)


2-sudo useradd -c "Bad User" -m baduser
sudo passwd baduser
![photo_5987695585202912751_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/ca414f9b-5a19-42ca-ba4a-9e5dfbe6a5c4)


3-sudo groupadd -g 30000 pgroup
![photo_5987695585202912753_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/f3c64952-16d7-4f6b-ba2b-1895c24354ce)

4-sudo groupadd -g 20000 badgroup
![photo_5987695585202912754_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/60d86067-8458-4a39-8b26-a538d0a1c691)


5-sudo usermod -aG pgroup islam
![photo_5987695585202912758_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/0dfd6b33-235f-45ec-b26a-8295274fdbbe)

6-sudo passwd islam

7-sudo chage -M 30 islam

8-sudo usermod -L baduser

9-sudo userdel -r baduser

10-sudo groupdel baduser

13-mkdir ~/myteam
chmod 400 ~/myteam

15-sudo cd ~/myteam

16-1-sudo touch oldpasswd
chmod u=rw,g=wx,o=x oldpasswd
chmod 711 oldpasswd

16-2-16 -2
Default permissions for files: 666 (rw-rw-rw-)
Default permissions for directories: 777 (rwxrwxrwx)

16-3-umask 077
mkdir testdir
touch test


