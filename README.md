RedHat
-------------------------------------------------------------------------
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

----------------------------------------------------------------------

Lab3
-----------
1- vi mycv

![photo_5987955207386021479_m](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/456e9062-385a-49ef-b1bc-4638105af8e8)


![photo_5987955207386021483_m](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/da029be5-bd95-4ceb-b60e-9f75fcb58cd4)

2- a. Move the cursor down one line at a time:

    Press j

b. Move the cursor up one line at a time:

    Press k

c. Search for the word "age":

    Type /age and press Enter

d. Step to line 5:

    Type :5 and press Enter

e. Delete the line you are on and line 5:

    Type dd to delete the current line
    Type :5 and press Enter to move to line 5
    Type dd to delete line 5

f. Step to the end of the line and change to writing mode in one step:

    Press $ to move to the end of the line
    Press A to enter insert mode at the end of the line
    
3-cat /etc/shells 

![photo_5987955207386021480_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/93ae7912-8d5b-4bc4-81cc-09340e023f79)


4-env

![photo_5987955207386021484_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/00192704-c53b-4957-b19c-133f5529e0f2)


5-printenv

![photo_5987955207386021485_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/3ebdbbae-098e-4396-9d4c-32eb23472f26)


6- echo $HOME

![photo_5987955207386021486_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/9c430d24-dcde-49e7-9c4d-d5fae275be3d)


7-echo $SHELL

![photo_5987955207386021487_m](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/864057ff-393b-4639-a8be-1f958cfb6552)

8-whereis sh
whereis ksh
whereis bash

![photo_5987955207386021488_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/060f32d6-056f-4aee-86c8-96a0c2f162d4)

9-nano ~/.bashrc
echo "Welcome, $(whoami)! Today is $(date)"

![photo_5987955207386021491_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/1646d7e3-4319-41f8-b9e9-31fb8fd0a6e3)


![photo_5987955207386021500_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/c16c5b37-6338-4423-8031-d6121977cd01)



10-    
enter echo \ and press Enter.
    The shell sees the backslash as an escape character, so it expects that the command is not complete and waits for more input.
    The shell shows a continuation prompt, which is often >, indicating that it's waiting for additional input to complete the command.

So, the continuation prompt (>) is telling you that the command you entered is not yet complete, and the shell is waiting for more input.

To change the continuation prompt from > to :, you can use the PS2 variable. This variable controls the secondary prompt (the continuation prompt). You can set it in your shell configuration file, such as ~/.bashrc. 

11-alias ls="ls -l"

![photo_5987955207386021492_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/64fb528a-cdf0-414f-8851-63eae6318ae9)

-------------------------------------------------------------------------------------------------------------------




Lab 5
-------

1-compress file
gzip -v file1
zip -v file2


![photo_5987695585202912951_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/afd55976-3cf3-4823-a41f-36058c2ce0a9)

file extention:
The compress command uses the .Z file extension for compressed files.
The gzip command uses the .gz file extension for compressed files.
The zip command creates a zip archive with the specified file(s) and uses the .zip extension.

-gzip is more widely supported and used on various platforms.
compress is less common today and may not be available by default on some systems.
-gzip has additional features, such as the ability to compress multiple files into a single archive (tar can be used in conjunction with gzip for this purpose).


2-zcat example.txt.gz

![photo_5987695585202912953_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/032d21de-5a53-4c93-9c8f-6e046885d0da)

3-tar -cvf ~/etc *

![photo_5987695585202912954_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/85d9662b-9178-432b-acba-36547ef004b7)


4-find ~/ -type f -mtime -2

![photo_5987695585202912955_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/2a469c72-1131-4e8a-ad9e-9f06cb65fa76)


5-sudo find /etc -type f -user root

![photo_5987695585202912958_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/e26bdcd0-d21d-4bc1-8aef-e7b9dd3b1f97)


6-find ~/ -type d

![photo_5987695585202912960_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/7c0e3f56-b454-4170-be7c-c4ff23448680)


7- sudo find / -type f -name ".profile"

![photo_5987695585202912961_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/cef49f34-6631-47b0-b0e1-c5bdae0bb97f)

8- file /etc/passwd
file /dev/pts/0
file /etc
file /dev/sda

![photo_5987955207386021496_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/8dbc6b97-ed74-4636-b898-41d962b25a93)


9- ls -i /
ls -i /etc
ls -i /etc/hosts

![photo_5987695585202912962_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/6fb8dffb-08ee-4d20-a0ab-ed021a6a37da)


![photo_5987695585202912963_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/bada2d7d-1367-4c63-ae53-fd3a7aaf8afb)


10-cp /etc/passwd ~/passwd_backup
diff /etc/passwd ~/passwd_backup
cmp /etc/passwd ~/passwd_backup

vi ~/passwd_backup
diff /etc/passwd ~/passwd_backup
cmp /etc/passwd ~/passwd_backup

![photo_5987955207386021503_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/34b98ecc-6e6b-4778-b544-b424e867487f)


11-sudo ln -s /etc/passwd /boot/passwd_link
ls -l /boot

![photo_5987955207386021509_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/125779d2-9c79-4852-84bb-d2e075cd2dee)



12- sudo ln /etc/passwd /boot/passwd_link
the /boot directory is on a different partition, you'll likely encounter an error message indicating that hard links across file
systems are not allowed.

![photo_5987955207386021511_y](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/cbb9a8eb-aed9-459d-8cb0-7591a6899fff)



ShellScript
------------------------
Lap1
-----
#sed

1-sed 'lp/p' /etc/passwd

![photo_5994743665190354553_y](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/88231d29-0f03-47f5-aaa5-9bd8df4da00e)



2-sed -e '3d' -e '1,$p' /etc/passwd

![photo_5994743665190354543_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/bd95442a-3ca5-4083-b285-9d719dd0eb58)


3-sed -e '$d' -e '1,$p' /etc/passwd

![photo_5994743665190354544_y](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/1f3c80ef-d5fa-466e-b600-2124edaa1324)


4-sed -e '/lp/d' -e '1,$p' /etc/passwd


![photo_5994743665190354564_y](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/99f49fb9-5945-48b9-bf8c-b9334aed987d)


5-sed 's/lp/mylp' /etc/passwd


![photo_5994743665190354549_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/d112431c-5f39-4572-9ea8-61db94e052c9)



#awk

1-awk -F: '{print $5}' /etc/passwd


![photo_5994743665190354572_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/b6bf6dd6-0ecb-4724-b397-883a3c7f31d3)


2-awk -F: '{print $1,$5,$6}' /etc/passwd

![photo_5994743665190354575_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/18b3f513-6b6d-4409-8a18-d7e24e1e1f69)


3-awk -F: '{ if($3>500) print $1,$3,$5}' /etc/passwd


![photo_5994743665190354578_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/c1c3bddb-56ba-4555-9589-1a0b6fd9b4a6)


4-awk -F: '{ if($3==500) print $1,$3,$5}' /etc/passwd


![photo_5994743665190354579_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/ce0ae42b-24ff-4359-9b00-7734310d3dda)


5-awk -F: '{ if(NR>=5&&NR<=15) print NR,$0}' /etc/passwd


![photo_5994743665190354598_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/914745ae-27f6-4705-94a2-54f8465630e6)


6-awk -F: '{for(i=1;i<=NF;i++) {if($i=="lp") $i="mylp"} print ;}' file1

![photo_5994743665190354604_y](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/d98aedc2-6c80-44db-bd81-f59405179c3e)


7-awk -F: 'BEGIN {max=0} {if ($3>max) {max=$3; maxline=$0}} END{print maxline}' file1


![photo_5994743665190354620_y](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/d99eedd0-8937-4557-a56f-4f4c84aeb584)


8-awk -F: 'BEGIN {sum=0} {sum+=$3} END {print sum}' file1

![photo_5994743665190354626_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/bcda9eff-8c4b-41a8-92af-36372a1db69d)


---------------------------------------------------------------------------------------------------------------------------
Lab3
---------------
1- 

![photo_5996948924738419950_w](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/bb2aef5e-092a-40c2-b6eb-265b8d9ca939)


2-

![photo_6017092385781169631_y](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/1b3722ca-0553-47ec-aff2-fa6eca2f5935)


![photo_6017092385781169634_m](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/0c8a122f-f8a9-44e8-9fb8-4bef1c814159)


3- 

![photo_6017092385781169676_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/f964e0c2-c7b4-438f-8998-6d3043943d5d)

![photo_6017092385781169677_y](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/7e6b2017-f1d8-4bf8-b35f-6c84ff2bbb68)


4- 

![photo_6017092385781169682_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/a08c0b74-7cbd-4fca-b06f-92f8e37b4342)

![photo_6017092385781169683_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/380f4534-692a-450d-b2c6-cfaf2b68bb70)


5- 

![photo_6017092385781169701_w](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/478872f9-19ae-4090-85db-c131019f2d16)


![photo_6017092385781169702_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/3ea718fd-7ddf-4d43-9144-3f33bdfb8814)


6-

![photo_6017092385781169705_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/ecf5103b-8232-4165-99b5-c368dd9853d5)



![photo_6017092385781169706_y](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/6bda37a4-1f1b-43b9-8257-a3c2b850e1d8)



![photo_6017092385781169707_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/f6a9436a-73d8-493a-bd1a-a5db145e83cf)










