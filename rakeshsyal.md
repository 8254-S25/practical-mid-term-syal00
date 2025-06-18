## CST 8254 Practical Mid Term

**Your Name:**

Rakesh Syal

student id : 041169281

Answer directly in this .md file.

### Task 1:

### Task 2:



Using ``scp`` , send a copy of the file to your raspberry pi in the home folder. **What command did you use?**

**1.**

```
scp rakeshsyal.txt pi@syal0005:/home/pi
```

Open a **`putty/ssh`** session to your raspberry pi .

**2. What command do you use to see a directory listing that includes the permissions of the files?**

```
ls -l

```

Redo the last command and save the output of the command to a file **`pr1.txt`**. **What command did you use?**

**3.**

```
  ls -l > pr1.txt

```

**4. What are the permissions of the file you just created?**

```
-rw-r--r-- 1 pi pi 516 Jun 18 11:15 pr1.txt
```

**5. What command do you use to display the folder you are currently working from?**

```
pwd

```

Change the permissions of the file so that group members can only execute it. **What command did you use?** 

**6.**

```
chmod 710 pr1.txt

```

Create a folder **`midtermExam-SectionNumber`** under the current working directory of your raspberry pi. **SectionNumber** must be replaced with your lab section number (for instance Jérôme's Lab students  use 301).  **What command did you use?**

**7.**

```
mkdir midtermExam-301
```

**8. What are the permissions of this new folder  ?**

```
drwxr-xr-x 2 pi pi 4096 Jun 18 11:21 midtermExam-301
```

**9. What command do you use to list the ports your raspberry pi is listening to? Try it using the `-at` flag.**

```
netstat -at

```

Redo the last command saving the output of the command to a file **`pr2.txt `**. **What command did you use?**

**10.**

```
netstat -at > pr2.txt

```



From the command line start a sFTP session to your raspberry PI . **What command did you use to connect?**

**11.**

```
sftp pi@10.0.0.116

```

Copy the file **`midtermPi.txt`** to your PI using sFtp. **What command did you use?** 

**12.**

```
put midtermPi.txt

```



**13.** What does the command do?

```
it shows nothing on pi but this command saves the current folder location into mt.txt, and adds a list of all files and folders into pr.txt.

```

Using `useradd`, create a user named after you using the concatenation of your firstname and last name. **What command did you use?**

**14.**

```
sudo useradd rakeshsyal

```

Create the home directory for the user you just created and change the ownership of this folder to the user himself/herself. **What commands did you use?**

 **15.**

```
 sudo mkdir /home/rakeshsyal
sudo chown rakeshsyal:rakeshsyal /home/rakeshsyal

```

Update your PI package list using `apt-get` , then use `apt-get` to install `Filezilla` on your  PI. **What commands did you use?**

**16.**

```
sudo apt-get update
sudo apt-get install filezilla -y

```

**17.** issue the following command on your pi:

`cd /home`

`ls -als > /home/pi/pr3.txt`










