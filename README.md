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
Q1
------


![photo_5996948924738419950_w](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/bb2aef5e-092a-40c2-b6eb-265b8d9ca939)




Q2
-----


![photo_6017092385781169631_y](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/1b3722ca-0553-47ec-aff2-fa6eca2f5935)


![photo_6017092385781169634_m](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/0c8a122f-f8a9-44e8-9fb8-4bef1c814159)


Q3
------


![photo_6017092385781169676_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/f964e0c2-c7b4-438f-8998-6d3043943d5d)



![photo_6017092385781169677_y](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/7e6b2017-f1d8-4bf8-b35f-6c84ff2bbb68)



Q4
-------


![photo_6017092385781169682_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/a08c0b74-7cbd-4fca-b06f-92f8e37b4342)



![photo_6017092385781169683_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/380f4534-692a-450d-b2c6-cfaf2b68bb70)


Q5
-------


![photo_6017092385781169701_w](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/478872f9-19ae-4090-85db-c131019f2d16)


![photo_6017092385781169702_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/3ea718fd-7ddf-4d43-9144-3f33bdfb8814)


Q6
------



![photo_6017092385781169705_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/ecf5103b-8232-4165-99b5-c368dd9853d5)



![photo_6017092385781169706_y](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/6bda37a4-1f1b-43b9-8257-a3c2b850e1d8)



![photo_6017092385781169707_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/f6a9436a-73d8-493a-bd1a-a5db145e83cf)




--------------------------------------------------------------------------------------------------------------------------
Lab3
------------------
Q1
------

![photo_6017203977621454736_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/3c902a5d-29dc-409f-93b8-5a0da2db0b36)



![photo_6017203977621454737_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/0e4517d2-55ea-42a9-8933-953dec704cc5)



Q2
-----


![photo_6017203977621454752_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/906db5d6-ad05-49ec-8d50-08441ae0695b)



![photo_6017203977621454753_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/e167e246-fe5f-46ae-9344-188dca3079f1)




Q3
-----

![photo_6017203977621454754_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/c13c6bfe-b0ac-4f18-aa69-b11300f4856b)



![photo_6017203977621454755_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/8c1f06ab-c764-4956-9703-06eeea04ed5c)




Q4
-----


![photo_6019141214030380630_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/8a9a4cd5-62aa-4e0d-b778-2fe784ff3a2a)



![photo_6019141214030380631_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/8580ec6e-428f-4151-a833-035a190901b1)



Q5
-----


![photo_6019141214030380634_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/dda43199-8958-428b-9064-5daed90a5ef8)



![photo_6019141214030380633_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/513056e3-d6f5-46c4-8447-028afe6a8868)



Q6
-------


![photo_6019141214030380636_y](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/30ec2460-0315-4413-8744-95c105765da3)



![photo_6019141214030380635_x](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/86dc383e-8fef-4ad2-89b8-0515e43804fd)


Q7
-------


![Screenshot from 2023-12-19 11-16-50](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/da80cc6d-019b-4001-95a3-6d2bbaa58420)



Q8
-------


![Screenshot from 2023-12-19 11-21-31](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/1d4adb07-e568-4423-8b0f-74c5ef26f15e)



Q9
--------



![Screenshot from 2023-12-19 11-25-35](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/73f34995-3de5-4934-a162-3b42508a7a5f)



Q10
-------



![Screenshot from 2023-12-19 11-30-22](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/87b37a30-5a3d-44ac-a725-a7c03fd74fc7)



Q11
--------



![Screenshot from 2023-12-19 11-35-22](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/7c791231-3166-4936-96dd-ef2916680188)




---------------------------------------------------------------------------------
Admin2
-------
Lab6
------
Q1:Use systemctl to view the status of all the system services.
---


![Screenshot from 2023-12-19 12-29-56](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/c7ce318f-6086-4998-830c-db5902b6832a)




Q2:Change the default run level back to multi-user.target and reboot.
---
sudo systemctl set-default multi-user.target


reboot .target


![Screenshot from 2023-12-19 14-42-34](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/9e56a3ac-2d16-4f79-9f25-39666920157d)



Q3:Send mail to the root user.
----


![Screenshot from 2023-12-19 14-55-11](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/5192a564-b403-47a7-846f-9cf71845a461)


Q4:Verify that you have received this mail.
---


![Screenshot from 2023-12-19 14-58-56](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/8ece5936-15c4-429a-96e5-ce3e766a3505)



Q5:Use  systemctl utility to stop postfix service
----


![Screenshot from 2023-12-19 15-01-54](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/7c93d514-c555-4ed5-ac8b-4f9b91d55546)



Q6:Send mail again to the root user.
------------


![Screenshot from 2023-12-19 15-07-04](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/bff4e8d8-4ee1-4bba-a66c-f02c6211a5f3)



Q7:Verify that you have received this mail.
--------


![Screenshot from 2023-12-19 15-09-01](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/ab012814-ddf2-4f83-bb1a-b3b9da150ebb)



Q8:Use systemctl utility to start postfix service
---------------


![Screenshot from 2023-12-19 15-12-06](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/fabeb52c-0be7-40c8-9c3a-3fe953e665ca)



Q9:Verify that you have received this mail
---------------


![Screenshot from 2023-12-20 08-47-54](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/b34db5d2-e9ea-434e-995e-f560ffd5e76c)



Q10:Edit in the GRUB2 configuration file and change the timeout variable equal 20 seconds.
------------------


![Screenshot from 2023-12-20 09-05-01](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/d4979662-aed2-4bf7-a89f-9e3b7a208cf2)



![Screenshot from 2023-12-20 09-05-22](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/f7de3acf-822c-4229-8316-47a4da6bc573)



Q11: Edit in the GRUB2 configuration file and change your default operating system
------------------------


![Screenshot from 2023-12-20 09-10-29](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/b2db5f6b-a14b-4ff5-8653-b0fb39954268)



Q12:You want to know some information about the status of the system every ten minutes today between the hours of  8:00 AM and 5:00 PM. to help investigate some performance issues you have been having. You suspect it might be memory related and want to keep an eye on those resources.
-----------------



![Screenshot from 2023-12-24 00-23-20](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/5fc11df1-d4a7-4c4a-bb0f-584086fe94b2)




Q13:Use mail as the root user to check for e-mail from the cron jobs you have scheduled.
-------------



![Screenshot from 2023-12-24 00-29-32](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/5317551f-5d81-4174-be99-e522c561bddc)




Q14:How could you send the output from these cron jobs to another e-mail address (the manager user)?
--------------------



![Screenshot from 2023-12-24 00-33-13](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/dfffc388-a2be-4ffd-9bb7-426e3d62c749)




Q15:Use mail as the manager user to check for e-mail from the cron jobs you have scheduled.
------------------------



![Screenshot from 2023-12-24 00-35-33](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/3a629c99-77ca-4dd0-8b86-86fd9dc1f312)





Q17:Attempt to run the command gnuplot. You should find that it is not
installed.
-------------------


![Screenshot from 2023-12-20 09-35-27](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/d974d522-8174-4cb3-9e12-4ae06905fb50)




Q18:Search for the plotting packages.
------------



![Screenshot from 2023-12-20 09-37-44](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/0c7c8538-2659-43a7-9bf3-e6ee4c98fb6b)




Q19:Find out more information about the gunuplot package.
-------------


![Screenshot from 2023-12-20 09-41-55](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/837b705e-5ef6-4c2d-bc7b-060259ed0e3d)



Q20:Install the gnuplot package.
-------------



![Screenshot from 2023-12-24 00-42-42](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/c8e940ae-559e-41a4-bdb5-11d076a4cd07)



Q21:Attempt to remove the gnuplot package, but say no
How many packages would be removed
------------------




![Screenshot from 2023-12-24 00-44-58](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/beab5c67-a44e-47da-877e-5f9d7aeef8d1)





Q22:List all installed packages in your system.
-------------------




![Screenshot from 2023-12-24 00-47-10](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/43b60c23-a9af-45bc-bc08-32e8999d9885)




Q23:View the files in the initscripts package
------------------


![Screenshot from 2023-12-24 00-49-55](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/2599bb34-e924-433d-956c-f0f5a107a54b)




Q24:Get general information about bash rpm.
----------------



![Screenshot from 2023-12-24 00-51-07](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/dab9afa0-d209-4952-89b4-b6dcd8b0248d)



Q25:Have the files from the pam package changed since it was
installed.
-----------------



![Screenshot from 2023-12-24 00-52-58](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/8a3b0938-5c29-4da0-aa88-dc8ba7855be3)




Q26:Which installed packages have gnome in their names?
-----------------



![Screenshot from 2023-12-24 00-54-53](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/531a56fa-fdcc-4d35-9592-92c793afa0eb)





------------------------------------------------------------------------------------------------------------
Lab 7
-------

Q1:Using the useradd command, add accounts for the following users in your system: user1, user2,
user3, user4, user5, user6 and user7. Remember to give each user a password.
-----------------


![Screenshot from 2023-12-24 01-02-09](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/1223ed84-90e4-466a-a1d7-4ecaa3da94ea)




Q2:Using the groupadd command, add the following groups to your system.
Group GID
sales 10000
hr 10001
web 10002
Why should you set GID in this manner instead of allowing the system to set the GID by default?
----------------



![Screenshot from 2023-12-24 01-06-04](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/3a61f50b-d73d-4176-9831-950454052042)






Q3:Using the usermod command to add user1 and user2 to the sales secondary group, user3 and user4
to the hr secondary group. User5 and user6 to web secondary group. And add user7 to all
secondary groups
------------------------------------



![Screenshot from 2023-12-24 01-10-44](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/b31f8578-ac41-4ee8-909a-cf15a3abfc55)



Q4:Login as each user and use id command to verify that they are in the appropriate groups. How else
might you verify this information?
----------------------




![Screenshot from 2023-12-24 01-15-56](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/30d5bb7d-5d60-4108-98d9-d6e44b8d2dbf)



Q5:Create a directory called /depts with a sales, hr, and web directory within the /depts directory.
-------------------



![Screenshot from 2023-12-24 01-18-34](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/932839c0-8608-4da2-a02e-526fb373923b)



Q6:Using the chgrp command, set the group ownership of each directory to the group with the
matching name
---------------------



![Screenshot from 2023-12-24 01-20-38](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/99dd020f-d975-495f-b8f5-f1b22c6946c1)




Q7:Set the permissions on the /depts directory to 755, and each subdirectory to 770
-----------------------



![Screenshot from 2023-12-24 01-22-37](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/1b328486-379c-4193-8e1a-09ca13e583cb)



Q8:Set the set-gid bit on each departmental directory
----------------------



![Screenshot from 2023-12-24 01-24-30](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/03318916-98c4-4680-9e95-6fe9f38c4ae3)



Q9:Use the su command to switch to the user2 account and attempt the following commands:
touch /depts/sales/user2.txt
touch /depts/hr/ user2.txt
touch /depts/web/ user2.txt
Which of these commands succeeded and which failed? What is the group ownership of the files
that were created?
------------------------




![Screenshot from 2023-12-24 01-28-50](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/09d1fd4d-2e0b-4ae0-b063-da61e4116976)




![Screenshot from 2023-12-24 01-29-38](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/08b72d3f-4904-413b-8b95-a147474de279)




Q10:Configure sudoers file to allow user3 and user4 to use /bin/mount and /bin/umount commands,
while allowing user5 only to use fdisk command.
--------------------


![Screenshot from 2023-12-24 01-32-18](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/676a3a4c-30ae-4804-93db-ff199e12570e)




Q11:Login by user3 and try to unmount /boot.
-----------



![Screenshot from 2023-12-24 01-34-16](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/3fe2b8dc-5095-4e80-8872-e7f6541f21de)




Q12:Login by user4 and remount /boot. Also try to view the partition table using fdisk.
------------------



![Screenshot from 2023-12-24 01-34-42](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/0b575bcf-715d-4a18-acc4-f4aafe470b09)




![Screenshot from 2023-12-24 01-37-37](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/c2389e00-ecdb-43bd-a0b2-a4d3e4b0ffed)




Q13:Create a directory with permissions rwxrwx---, grant a second group (sales) r-x permissions
-------------------------



![Screenshot from 2023-12-24 01-42-20](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/9b5d6995-cd91-4183-9546-b0a7a7b3bcee)




Q14:create a file on that directory and grant read and write to a second group (sales)
---------------------



![Screenshot from 2023-12-24 01-46-43](https://github.com/fatmaelhot/ITI_RedHat/assets/128849238/8b7ccd1d-696c-4f79-91a8-ef9eb51cea80)


