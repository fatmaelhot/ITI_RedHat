LAP 1
-----------------------------------------------------------
2-cat: scroll off and display the end of pages
more: display output one screen at one time (page by page) 
3-rm: to remove files
rmdir: to remove directory 
4-/home --> mkdir dir1 doc
/home/dir1 --> mkdir dir11 dir12

![photo_5987695585202912862_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/a9e3c039-04bd-48e0-8bea-292b651e86f4)

/home/doc --> touch mycv
/home/dir1/dir11/ --> touch file1

![photo_5987695585202912863_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/53d2ab06-ea20-4b42-bb2d-9a6b94feba84)


4-a-rmdir dir11


![photo_5987695585202912865_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/fff4e6a4-0869-40d4-9b98-8312af216aeb)

4-b- rmdir -p

![photo_5987695585202912866_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/5bcad883-c96c-42c2-ba8f-036252161ddf)

4-c- home
./home

5-cp etc/passwod  home/mypasswod

![photo_5987695585202912867_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/7235853e-4042-41ae-a5c4-c0f646b62b8d)

6-mv mypasswd oldpasswd

![photo_5987695585202912868_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/613c7162-3750-4bc2-b508-026e14b5d0a2)

7-../../home or cd /home   or cd ~home or cd-home 
8-ls /usr/bin/w*

![photo_5987695585202912871_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/2e36b98a-08bd-4090-bb31-8c21d119a715)

9-head -n 4 /etc/passwd

![photo_5987695585202912872_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/f0888c07-4a44-4725-a1c5-79f27644b490)

10-tail -n 7 /etc/passwd

![photo_5987695585202912873_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/dcae9714-a25c-44b4-beef-f61d786b3cf5)

11- man passwd && cat /etc/passwd

![photo_5987695585202912874_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/e80bed60-6c34-4708-87cc-3ed17768c63f)

12-man 5 passwd

![photo_5987695585202912875_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/e6036247-92a0-4f16-b49e-5a9462b03614)

13-man -K passwd


![photo_5987695585202912877_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/940396e5-75f3-43b2-8d58-1b907956aa0a)


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

![photo_5987695585202912759_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/e9503064-90c1-436a-a5ca-5b5592bd0672)


7-sudo chage -M 30 islam

![photo_5987695585202912761_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/0207c153-e8b4-4da3-8751-027ded9594ba)

8-sudo usermod -L baduser

![photo_5987695585202912762_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/daea4947-1149-4a15-adf4-177a8cd35d8f)

9-sudo userdel -r baduser

![photo_5987695585202912766_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/72a7bd16-726a-4263-b7cb-9f975651519f)


10-sudo groupdel baduser


![photo_5987695585202912769_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/342fd8ed-dadd-47c7-bcff-2de1a1e66634)


13-mkdir ~/myteam
chmod 400 ~/myteam

![photo_5987695585202912771_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/cbaf5350-aeb6-4cc1-90af-54de90a1156f)

14-su islam

![photo_5987695585202912792_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/efbf2a4e-2277-4d6a-8504-41903f19c834)


15-sudo cd ~/myteam

![photo_5987695585202912775_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/53d3ffd9-4d14-4a70-9eea-d5d9d16ee9d1)


16-1-sudo touch oldpasswd
chmod u=rw,g=wx,o=x oldpasswd
chmod 711 oldpasswd

![photo_5987695585202912780_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/314d296b-1f8c-4e15-81ac-b334820413fb)


16-2-16 -2
Default permissions for files: 666 (rw-rw-rw-)
Default permissions for directories: 777 (rwxrwxrwx)

16-3-umask 077
mkdir testdir
touch test

![photo_5987695585202912782_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/63fd8480-f323-44ab-b781-2fe0f1107d63)



