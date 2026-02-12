# OS-Linux-commands-Shell-scripting
Operating systems Lab exercise
# Linux commands-Shell scripting
Linux commands-Shell scripting

# AIM:
To practice Linux Commands and Shell Scripting

# DESIGN STEPS:

### Step 1:

Navigate to any Linux environment installed on the system or installed inside a virtual environment like virtual box/vmware or online linux JSLinux (https://bellard.org/jslinux/vm.html?url=alpine-x86.cfg&mem=192) or docker.

### Step 2:

Execute the following commands

### Step 3:

Testing the commands for the desired output. 

# COMMANDS:
### Create the following files file1, file2 as follows:
cat > file1
```
chanchal singhvi
c.k. shukla
s.n. dasgupta
sumit chakrobarty
^d
```
<img width="479" height="136" alt="Screenshot from 2026-02-06 09-27-14" src="https://github.com/user-attachments/assets/6c59d312-11bd-461d-8c25-ab2237d008a4" />

cat > file2
```
anil aggarwal
barun sengupta
c.k. shukla
lalit chowdury
s.n. dasgupta
^d
```
<img width="479" height="136" alt="Screenshot from 2026-02-06 09-29-03" src="https://github.com/user-attachments/assets/d720efce-a2ab-4092-a77c-285e9e8b4622" />


### Display the content of the files
cat < file1
## OUTPUT
<img width="478" height="127" alt="Screenshot from 2026-02-06 09-29-52" src="https://github.com/user-attachments/assets/6888ab5a-1218-4dad-8e6d-7acacfee85d4" />

cat < file2

## OUTPUT

<img width="478" height="127" alt="Screenshot from 2026-02-06 09-29-32" src="https://github.com/user-attachments/assets/d2578a82-5272-4925-882a-d7dd72294ce5" />


# Comparing Files
cmp file1 file2
## OUTPUT
 <img width="477" height="73" alt="Screenshot from 2026-02-06 09-30-30" src="https://github.com/user-attachments/assets/18dc6e09-aaef-49da-bf4b-d6d619311cae" />

comm file1 file2
 ## OUTPUT
<img width="510" height="292" alt="Screenshot from 2026-02-06 09-30-57" src="https://github.com/user-attachments/assets/e11c74fd-a4eb-416e-9210-3d3da0f03ec4" />

 
diff file1 file2
## OUTPUT
<img width="510" height="292" alt="Screenshot from 2026-02-06 09-31-13" src="https://github.com/user-attachments/assets/266f508c-4de3-4473-af43-00fd5c4b1ea2" />


#Filters

### Create the following files file11, file22 as follows:

cat > file11
```
Hello world
This is my world
^d
```
<img width="513" height="98" alt="Screenshot from 2026-02-06 09-32-20" src="https://github.com/user-attachments/assets/0443ff17-fe7a-44b0-8395-102f73e87e45" />

cat > file22
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
^d
```
<img width="513" height="97" alt="Screenshot from 2026-02-06 09-35-39" src="https://github.com/user-attachments/assets/0ac1f51c-975d-4f6d-b2ad-c964ecef67df" />


cut -c1-3 file11
## OUTPUT

<img width="512" height="85" alt="Screenshot from 2026-02-06 09-36-37" src="https://github.com/user-attachments/assets/42214f54-4fb3-452a-9e34-0c65ad72b82e" />



cut -d "|" -f 1 file22
## OUTPUT



cut -d "|" -f 2 file22
## OUTPUT
<img width="538" height="100" alt="Screenshot from 2026-02-06 09-37-52" src="https://github.com/user-attachments/assets/06655e4e-a024-4d88-a682-47288e986404" />


cat < newfile 
```
Hello world
hello world
^d
````
<img width="467" height="51" alt="Screenshot from 2026-02-09 08-33-41" src="https://github.com/user-attachments/assets/a183a14f-9312-42dd-8963-9f364477468d" />


cat > newfile 
Hello world
hello world

<img width="462" height="78" alt="Screenshot from 2026-02-09 08-33-31" src="https://github.com/user-attachments/assets/4f180e6e-e00a-49ed-915c-b9a9862c3de0" />

 
grep Hello newfile 
## OUTPUT

<img width="506" height="51" alt="Screenshot from 2026-02-09 08-40-52" src="https://github.com/user-attachments/assets/d5dd2dd0-252e-484b-ac7b-82094304fc67" />


grep -v hello newfile 
## OUTPUT
<img width="542" height="51" alt="Screenshot from 2026-02-09 08-41-36" src="https://github.com/user-attachments/assets/b53cba0a-986b-4c9c-a826-c051d3fa1064" />


cat newfile | grep -i "hello"
## OUTPUT

<img width="625" height="74" alt="Screenshot from 2026-02-09 08-47-38" src="https://github.com/user-attachments/assets/226c572d-d64a-46b8-b757-130ba17aa3ea" />


cat newfile | grep -i -c "hello"
## OUTPUT


<img width="625" height="74" alt="Screenshot from 2026-02-09 08-47-53" src="https://github.com/user-attachments/assets/ffcbe3e9-c91a-46f9-863a-fc5f0c168f1b" />


grep -R ubuntu /etc
## OUTPUT

<img width="1197" height="389" alt="Screenshot from 2026-02-09 08-45-13" src="https://github.com/user-attachments/assets/4770a1f6-3137-4d76-b707-f08a495aa2b1" />


grep -w -n world newfile   
## OUTPUT
<img width="625" height="74" alt="Screenshot from 2026-02-09 08-54-03" src="https://github.com/user-attachments/assets/538455c8-0cd3-4729-974c-6b1d60a0f0c0" />


cat < newfile 
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
```
<img width="622" height="128" alt="Screenshot from 2026-02-09 08-56-17" src="https://github.com/user-attachments/assets/e228d53d-b900-497e-9df8-86f44392c954" />

cat > newfile
```
Hello world
hello world
Linux is world number 1
Unix is predecessor
Linux is best in this World
^d
 ```
<img width="622" height="128" alt="Screenshot from 2026-02-09 08-56-09" src="https://github.com/user-attachments/assets/de781c65-2ea7-4342-847e-311c78023ac3" />


egrep -w 'Hello|hello' newfile 
## OUTPUT

<img width="623" height="61" alt="Screenshot from 2026-02-09 08-57-00" src="https://github.com/user-attachments/assets/1413e2f4-67f5-4b82-a64a-61c4c5fd9e48" />

egrep -w '(H|h)ell[a-z]' newfile 
## OUTPUT

<img width="623" height="61" alt="Screenshot from 2026-02-09 08-57-51" src="https://github.com/user-attachments/assets/6b3a3128-2064-4cd2-91d4-40d409ed1044" />



egrep '(^hello)' newfile 
## OUTPUT

<img width="623" height="61" alt="Screenshot from 2026-02-09 08-58-18" src="https://github.com/user-attachments/assets/59dd98dc-b9f1-4f57-a70c-19079aebb599" />



egrep '(world$)' newfile 
## OUTPUT

<img width="621" height="100" alt="Screenshot from 2026-02-09 08-58-58" src="https://github.com/user-attachments/assets/8cb55ca8-9cf9-4842-9a08-05bfaa29efb7" />

egrep '((W|w)orld$)' newfile 
## OUTPUT

<img width="621" height="100" alt="Screenshot from 2026-02-09 09-00-05" src="https://github.com/user-attachments/assets/c01ab1cc-317d-43f7-b030-89b2bc8f9c59" />


egrep '[1-9]' newfile 
## OUTPUT

<img width="620" height="69" alt="Screenshot from 2026-02-09 09-00-36" src="https://github.com/user-attachments/assets/bf6326a8-f0fb-45a6-84bd-0407a45e693b" />


egrep 'Linux.*world' newfile 
## OUTPUT
<img width="643" height="45" alt="image" src="https://github.com/user-attachments/assets/3659cb12-27ed-4564-ab79-e21ac365f994" />


egrep 'Linux.*World' newfile 
## OUTPUT
<img width="643" height="45" alt="image" src="https://github.com/user-attachments/assets/0ff903f6-35d5-4562-96e0-608a0167dbb6" />


egrep l{2} newfile
## OUTPUT

<img width="643" height="57" alt="image" src="https://github.com/user-attachments/assets/57da793e-c5a9-4943-ba62-5fe67cd5e0f2" />


egrep 's{1,2}' newfile
## OUTPUT 
<img width="643" height="75" alt="image" src="https://github.com/user-attachments/assets/6ab78674-1fee-4208-bd8b-6c833d7316bb" />


cat > file23
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
1003 | Joe |  7000 | Developer
1001 | Ram | 10000 | HR
^d
```


sed -n -e '3p' file23
## OUTPUT

<img width="643" height="46" alt="image" src="https://github.com/user-attachments/assets/ac239b1a-6d05-4faa-8d8e-84dfcfac0af4" />


sed -n -e '$p' file23
## OUTPUT

<img width="643" height="39" alt="image" src="https://github.com/user-attachments/assets/abab11d3-fc6c-4b8f-92cf-e01ac3da4c7d" />


sed  -e 's/Ram/Sita/' file23
## OUTPUT

<img width="643" height="169" alt="image" src="https://github.com/user-attachments/assets/993bc113-dfda-4009-8f78-c7b474d5b13e" />


sed  -e '2s/Ram/Sita/' file23
## OUTPUT

<img width="643" height="169" alt="image" src="https://github.com/user-attachments/assets/0f4a63ab-6a3a-4f81-b8ce-f0916c2067d9" />



sed  '/tom/s/5000/6000/' file23
## OUTPUT
<img width="643" height="169" alt="image" src="https://github.com/user-attachments/assets/81f43626-742d-46be-b781-83772072091b" />



sed -n -e '1,5p' file23
## OUTPUT

<img width="643" height="113" alt="image" src="https://github.com/user-attachments/assets/e910ee17-19e4-4f4e-a00d-3179df59c8ff" />


sed -n -e '2,/Joe/p' file23
## OUTPUT

<img width="643" height="77" alt="image" src="https://github.com/user-attachments/assets/4fca73e2-d756-4127-a678-cb44b7655f66" />



sed -n -e '/tom/,/Joe/p' file23
## OUTPUT

<img width="643" height="60" alt="image" src="https://github.com/user-attachments/assets/1219a296-14a7-425c-a869-6c34fb053750" />


seq 10 
## OUTPUT

<img width="643" height="203" alt="image" src="https://github.com/user-attachments/assets/13d326c2-09fc-4d59-ade2-a2404383a219" />


seq 10 | sed -n '4,6p'
## OUTPUT

<img width="643" height="75" alt="image" src="https://github.com/user-attachments/assets/c3e2bb1d-a2bb-45fe-be36-27ad9f5cc92b" />


seq 10 | sed -n '2,~4p'
## OUTPUT

<img width="643" height="75" alt="image" src="https://github.com/user-attachments/assets/89ab9237-e589-4388-9bf2-17982037ccfe" />


seq 3 | sed '2a hello'
## OUTPUT

<img width="643" height="94" alt="image" src="https://github.com/user-attachments/assets/99f1eab4-7325-4aa0-9366-cc26359c9667" />


seq 2 | sed '2i hello'
## OUTPUT

<img width="643" height="83" alt="image" src="https://github.com/user-attachments/assets/1cd93ddf-0876-4e1c-9166-a2a4345f0f9f" />

seq 10 | sed '2,9c hello'
## OUTPUT

<img width="643" height="80" alt="image" src="https://github.com/user-attachments/assets/7a370211-829a-4ec4-8241-e9280db420d0" />

sed -n '2,4{s/^/$/;p}' file23
## OUTPUT

<img width="643" height="90" alt="image" src="https://github.com/user-attachments/assets/119eacc1-c5af-41ce-a0cd-123335e5ec38" />


sed -n '2,4{s/$/*/;p}' file23

<img width="643" height="77" alt="image" src="https://github.com/user-attachments/assets/3c2f9a07-4d95-44aa-8fb3-e2fe8ce2c81e" />

#Sorting File content
cat > file21
```
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
sort file21
## OUTPUT

<img width="643" height="93" alt="image" src="https://github.com/user-attachments/assets/ccd2b849-5fb1-446e-a988-13ba8ec41019" />

cat > file22
```
1001 | Ram | 10000 | HR
1001 | Ram | 10000 | HR
1002 | tom |  5000 | Admin
1003 | Joe |  7000 | Developer
1005 | Sam |  5000 | HR
1004 | Sit |  7000 | Dev
``` 
uniq file22
## OUTPUT

<img width="643" height="115" alt="image" src="https://github.com/user-attachments/assets/60ace510-7a94-4ca7-b99c-d33101dbbe18" />


#Using tr command

cat file23 | tr [:lower:] [:upper:]
 ## OUTPUT

<img width="677" height="166" alt="image" src="https://github.com/user-attachments/assets/a5eff68c-8244-4b7b-be9a-06b1a51d8171" />

cat < urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
^d
 ```
cat > urllist.txt
```
www. yahoo. com
www. google. com
www. mrcet.... com
 ```
cat urllist.txt | tr -d ' '
 ## OUTPUT

<img width="677" height="85" alt="image" src="https://github.com/user-attachments/assets/17eb480d-03f6-4ea4-b3f6-ed0ecf9387b8" />

 
cat urllist.txt | tr -d ' ' | tr -s '.'
## OUTPUT

<img width="728" height="79" alt="image" src="https://github.com/user-attachments/assets/d4b7d071-b4bb-41aa-aeb8-937b4d0839ee" />


#Backup commands
tar -cvf backup.tar *
## OUTPUT

<img width="863" height="157" alt="image" src="https://github.com/user-attachments/assets/311083e2-3db9-4158-9c4d-4e048ee3004e" />

mkdir backupdir
 
mv backup.tar backupdir

cd backupdir
 
tar -tvf backup.tar
## OUTPUT

<img width="844" height="204" alt="image" src="https://github.com/user-attachments/assets/1981a374-23b1-4335-80c6-b90f7020b9ab" />


tar -xvf backup.tar
## OUTPUT
<img width="518" height="200" alt="image" src="https://github.com/user-attachments/assets/84db2cb2-5630-4177-8107-e1fa94a8ef95" />

gzip backup.tar

ls .gz
## OUTPUT

<img width="518" height="44" alt="image" src="https://github.com/user-attachments/assets/28f0930d-be0a-47cb-905c-85fa70d218aa" />

 
gunzip backup.tar.gz
## OUTPUT

<img width="704" height="308" alt="image" src="https://github.com/user-attachments/assets/eb0544bd-4371-4ac2-b8a8-cf07c47e257a" />


# Shell Script
```
echo '#!/bin/sh' > my-script.sh
echo 'echo Hello World‘; exit 0 >> my-script.sh
```
chmod 755 my-script.sh
./my-script.sh
## OUTPUT

<img width="529" height="48" alt="image" src="https://github.com/user-attachments/assets/7f15bb9e-0759-4798-a6d5-120b3f9f6976" />

 
cat << stop > herecheck.txt
```
hello in this world
i cant stop
for this non stop movement
stop
```

cat herecheck.txt
## OUTPUT

<img width="532" height="63" alt="image" src="https://github.com/user-attachments/assets/9dde414b-0a7f-4f59-b498-8b5d2cd89231" />

cat < scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $1#
echo 'The $$ is ' $$
ps
^d
 ```

cat scriptest.sh 
```bash
\#!/bin/sh
echo “File name is $0 ”
echo "File name is " `basename $0`
echo “First arg. is ” $1
echo “Second arg. is ” $2
echo “Third arg. is ” $3
echo “Fourth arg. is ” $4
echo 'The $@ is ' $@
echo 'The $\# is ' $\#
echo 'The $$ is ' $$
ps
```
 
chmod 777 scriptest.sh
 
./scriptest.sh 1 2 3

## OUTPUT

<img width="571" height="345" alt="image" src="https://github.com/user-attachments/assets/15d77f6e-81b2-4eb7-9566-acd59e912126" />

 
ls file1
## OUTPUT

<img width="571" height="49" alt="image" src="https://github.com/user-attachments/assets/2dfeef32-574f-40ef-bdda-44ffab8d9c15" />


echo $?
## OUTPUT 
<img width="571" height="43" alt="image" src="https://github.com/user-attachments/assets/216cab34-9409-4e5f-805f-dde2b989251d" />


./one
bash: ./one: Permission denied
 
echo $?
## OUTPUT 

 <img width="571" height="43" alt="image" src="https://github.com/user-attachments/assets/e37bacdd-2769-4342-a75f-00066b4bb2c3" />

abcd
 
echo $?
 ## OUTPUT

<img width="571" height="43" alt="image" src="https://github.com/user-attachments/assets/674531be-53b4-488e-875d-f085176e4f0d" />

 
# mis-using string comparisons

cat < strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
^d
```

cat strcomp.sh 
```bash
\#!/bin/bash
val1=baseball
val2=hockey
if [ $val1 \> $val2 ]
then
echo "$val1 is greater than $val2"
else
echo "$val1 is less than $val2"
fi
```
chmod 755 strcomp.sh
 
./strcomp.sh 
## OUTPUT

<img width="571" height="62" alt="image" src="https://github.com/user-attachments/assets/4a259305-ecd7-49e0-899a-c19b5724613a" />


# check file ownership
cat < psswdperm.sh 
```bash
\#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
^d
```

cat psswdperm.sh 
```bash
/#!/bin/bash
if [ -O /etc/passwd ]
then
echo “You are the owner of the /etc/passwd file”
else
echo “Sorry, you are not the owner of the /etc/passwd file”
fi
 ```
./psswdperm.sh
## OUTPUT

<img width="593" height="61" alt="image" src="https://github.com/user-attachments/assets/7ff12f1d-27fd-4080-8a44-8f1ce4021e8e" />


# check if with file location
cat>ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d
```
cat ifnested.sh 
```
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```

./ifnested.sh 
## OUTPUT

<img width="812" height="114" alt="image" src="https://github.com/user-attachments/assets/146fcc96-56a5-4f84-b4ce-c36ffc82b46a" />


# using numeric test comparisons
cat > iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
^d
```


cat iftest.sh 
```bash
\#!/bin/bash
val1=10
val2=11
if [ $val1 -gt 5 ]
then
echo “The test value $val1 is greater than 5”
fi
if [ $val1 -eq $val2 ]
then
echo “The values are equal”
else
echo “The values are different”
fi
```

$ chmod 755 iftest.sh
 
$ ./iftest.sh 
## OUTPUT

<img width="812" height="114" alt="image" src="https://github.com/user-attachments/assets/1881d1a8-220d-453f-a949-8498bee4d922" />


# check if a file
cat > ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
^d
```

cat ifnested.sh 
```bash
\#!/bin/bash
if [ -e $HOME ]
then
echo “$HOME The object exists, is it a file?”
if [ -f $HOME ]
then
echo “Yes,$HOME it is a file!”
else
echo “No,$HOME it is not a file!”
if [ -f $HOME/.bash_history ]
then
echo “But $HOME/.bash_history is a file!”
fi
fi
else
echo “Sorry, the object does not exist”
fi
```

$ chmod 755 ifnested.sh
 
$ ./ifnested.sh 
## OUTPUT

<img width="812" height="114" alt="image" src="https://github.com/user-attachments/assets/9c66ee97-1b6b-4c2e-a5e5-cc9c121513df" />


# looking for a possible value using elif
cat elifcheck.sh 
```bash
\#!/bin/bash
if [ $USER = Ram ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Rahim ]
then
echo "Welcome $USER"
echo "Please enjoy your visit"
elif [ $USER = Robert ]
then
echo "Special testing account"
elif [ $USER = gganesh ]
then
echo "$USER, Do not forget to logout when you're done"
else
echo "Sorry, you are not allowed here"
fi
```

$ chmod 755 elifcheck.sh
 
$ ./elifcheck.sh 
## OUTPUT


<img width="812" height="79" alt="image" src="https://github.com/user-attachments/assets/04cd6021-7bca-4941-8ccf-2085bb76bd90" />


# testing compound comparisons
cat> ifcompound.sh 
```bash
\#!/bin/bash
if [ -d $HOME ] && [ -w $HOME ]
then
echo "The file exists and you can write to it"
else
echo "I cannot write to the file"
fi
```
$ chmod 755 ifcompound.sh
$ ./ifcompound.sh 
## OUTPUT

<img width="812" height="79" alt="image" src="https://github.com/user-attachments/assets/1919690b-bb32-440c-b611-0c6bca73defe" />


# using the case command
cat >casecheck.sh 
```bash
case $USER in
Ram | Robert)
echo "Welcome, $USER"
echo "Please enjoy your visit";;
Rahim)
echo "Special testing account";;
gganesh)
echo "$USER, Do not forget to log off when you're done";;
*)
echo "Sorry, you are not allowed here";;
esac
```
$ chmod 755 casecheck.sh 
 
$ ./casecheck.sh 

 ## Output
 
 <img width="728" height="79" alt="image" src="https://github.com/user-attachments/assets/bcde60e1-3dd9-4962-876b-3c89d316c7e8" />

 
cat > whiletest
```bash
#!/bin/bash
#while command test
var1=10
while [ $var1 -gt 0 ]
do
echo $var1
var1=$[ $var1 - 1 ]
done
```
$ chmod 755 whiletest.sh
 
$ ./whiletest.sh

 ## output

 <img width="595" height="133" alt="image" src="https://github.com/user-attachments/assets/834c2ee8-9a67-4b91-adcb-31602c009be0" />

 
cat untiltest.sh 
```bash
\#using the until command
var1=100
until [ $var1 -eq 0 ]
do
echo $var1
var1=$[ $var1 - 25 ]
done
``` 
$ chmod 755 untiltest.sh
## OUTPUT

<img width="595" height="133" alt="image" src="https://github.com/user-attachments/assets/8e74640a-df93-4373-8de2-ccfefd0a4f02" />

 
cat forin1.sh 
```bash
\#!/bin/bash
\#basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
 ```
 
$ chmod 755 forin1.sh
 
 
cat forin2.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
 ```
 
$ chmod 755 forin2.sh
 
cat forin2.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don't know if this'll work
do
echo “word:$test”
done
```
$ chmod 755 forin2.sh
 
$ ./forin2.sh 
 
cat forin3.sh 
```bash
\#!/bin/bash
\# another example of how not to use the for command
for test in I don\'t know if "this'll" work
do
echo "word:$test"
done
```
$ ./forin3.sh 
 
cat forin1.sh 
```bash
#!/bin/bash
# basic for command
for test in Alabama Alaska Arizona Arkansas California Colorado
do
echo The next state is $test
done
```
$ chmod 755 forin1.sh

## OUTPUT

<img width="595" height="167" alt="image" src="https://github.com/user-attachments/assets/431b8ef9-d731-4203-a183-9ac0ff44a0d3" />


cat forinfile.sh 
```bash
#!/bin/bash
# reading values from a file
file="cities"
for state in `cat $file`
do
echo "Visit beautiful $file“
done
```
$ chmod 777 forinfile.sh
$ cat cities
Hyderabad
Alampur
Basara
Warangal
Adilabad
Bhadrachalam
Khammam

## OUTPUT

<img width="595" height="133" alt="image" src="https://github.com/user-attachments/assets/5c7d6a29-ce31-4fc7-aa49-904f7048bb40" />

cat forctype.sh 
```bash
#!/bin/bash
# testing the C-style for loop
for (( i=1; i <= 5; i++ ))
do
echo "The value of i is $i"
done
````
$ chmod 755 forctype.sh
$ ./forctype.sh 
## OUTPUT

<img width="595" height="133" alt="image" src="https://github.com/user-attachments/assets/54955715-6e5c-4576-8d9a-54c86ca8dffd" />


cat forctype1.sh 
```bash
#!/bin/bash
# multiple variables
for (( a=1, b=5; a <= 5; a++, b-- ))
do
echo "$a - $b"
done
```
$ chmod 755 forctype.sh
$ ./forctype1.sh 
## OUTPUT

<img width="595" height="255" alt="image" src="https://github.com/user-attachments/assets/ae11296c-2bcd-47b8-8735-14653b724f1c" />


cat fornested1.sh 
```bash
#!/bin/bash
# nesting for loops
for (( a = 1; a <= 3; a++ ))
do
echo "Starting loop $a:"
for (( b = 1; b <= 3; b++ ))
do
echo " Inside loop: $b"
done
done
```
$ chmod 755 fornested1.sh
 
$ ./fornested1.sh 
 ## OUTPUT

 <img width="595" height="255" alt="image" src="https://github.com/user-attachments/assets/7fa3f2df-ce8e-4ea6-a6cd-1cf1191ddfc9" />

cat forbreak.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
break
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“
```
## OUTPUT

<img width="595" height="96" alt="image" src="https://github.com/user-attachments/assets/22071924-ebe5-48cb-9fa3-d69be0558d70" />


$ chmod 755 forbreak.sh
 
$ ./forbreak.sh 
 
cat forbreak.sh 
```bash
#!/bin/bash
# breaking out of a for loop
for var1 in 1 2 3 4 5
do
if [ $var1 -eq 3 ]
then
continue
fi
echo "Iteration number: $var1"
done
echo "The for loop is completed“
```

 
$ chmod 755 forcontinue.sh
 
$ ./forcontinue.sh 
## OUTPUT
 <img width="595" height="78" alt="image" src="https://github.com/user-attachments/assets/a6557735-efa1-4996-bd89-f3712a4e24a8" />

cat exread.sh 
```bash
#!/bin/bash
# testing the read command
echo -n "Enter your name: "
read name
echo "Hello $name, welcome to my program. "
 ```
 
$ chmod 755 exread.sh 
 
$ ./exread.sh 
## OUTPUT

<img width="595" height="78" alt="image" src="https://github.com/user-attachments/assets/35ece021-40f8-4096-bbe0-d2177bbc037d" />


 cat exread1.sh
```bash
#!/bin/bash
# testing the read command
read -p "Enter your name: " name
echo "Hello $name, welcome to my program. “
``` 
$ chmod 755 exread1.sh 

## OUTPUT

<img width="595" height="59" alt="image" src="https://github.com/user-attachments/assets/8213b892-d3ef-4b5c-a2eb-08bb1a9911f0" />


$ ./exread1.sh 
 
cat funcex.sh
```bash
#!/bin/bash
# trying to access script parameters inside a function
function func {
echo $[ $1 * $2 ]
}
if [ $# -eq 2 ]
then
value=`func $1 $2`
echo "The result is $value"
else
echo "Usage: badtest1 a b"
fi
```
## OUTPUT

<img width="595" height="59" alt="image" src="https://github.com/user-attachments/assets/233bdc56-5339-4bb0-a9fa-dac9c1d6772e" />


 ./funcex.sh 

 
 ./funcex.sh 1 2

 ## OUTPUT

 <img width="595" height="41" alt="image" src="https://github.com/user-attachments/assets/c678631c-b0b0-42cc-90e7-ee18bb1396e8" />


 
cat argshift.sh
```bash
#!/bin/bash 
 while (( "$#" )); do 
  echo $1 
  shift 
done
```
$ chmod 777 argshift.sh

## OUTPUT

<img width="595" height="76" alt="image" src="https://github.com/user-attachments/assets/46bf1b6b-c8f2-4d7a-9e6c-230f6993bdc0" />


$ ./argshift.sh 1 2 3
 
 cat argshift1.sh
```bash
 #/bin/bash 
 # store arguments in a special array 
args=("$@") 
# get number of elements 
ELEMENTS=${#args[@]} 
 # echo each element in array  
# for loop 
for (( i=0;i<$ELEMENTS;i++)); do 
    echo ${args[${i}]} 
done
```
$ chmod 777 argshift.sh
## OUTPUT

<img width="595" height="76" alt="image" src="https://github.com/user-attachments/assets/8f9badab-b881-4d86-adff-6e411163bc70" />


$ ./argshift.sh 1 2 3
 
cat argshift.sh
```bash
#!/bin/bash 
set -x 
while (( "$#" )); do 
  echo $1 
  shift 
done
set +x
```
## OUTPUT

<img width="595" height="291" alt="image" src="https://github.com/user-attachments/assets/e80b2f86-00db-4ebd-b5c6-c804295f8ff2" />


 ./argshift.sh 1 2 3
 
 
cat > nc.awk
```bash
BEGIN{}
{
print len=length($0),"\t",$0 
wordcount+=NF
chrcnt+=len
}
END {
print "total characters",chrcnt 
print "Number of Lines are",NR
print "No of Words count:",wordcount
}
 ```
cat>data.dat
```bash
bcdfghj
abcdfghj
bcdfghj
ebcdfghj
bcdfghj
ibcdfghj
bcdfghj
obcdfghj
bcdfghj
ubcdfghj
```
awk -f nc.awk data.dat
## OUTPUT 

 <img width="559" height="281" alt="image" src="https://github.com/user-attachments/assets/82742db5-9bb2-47ae-86cd-d3074a506b20" />

cat > palindrome.sh
```bash
#num=545
echo "Enter the number"
read num
s=0
rev=""
temp=$num
while [ $num -gt 0 ]
do
	# Get Remainder
	s=$(( $num % 10 ))
	# Get next digit
	num=$(( $num / 10 ))
	# Store previous number and
	# current digit in reverse
	rev=$( echo ${rev}${s} )
done
if [ $temp -eq $rev ];
then
	echo "Number is palindrome"
else
	echo "Number is NOT palindrome"
fi
```
## OUTPUT 

<img width="599" height="112" alt="image" src="https://github.com/user-attachments/assets/c9969ac5-000e-4ba7-b7a6-17982caeb8ad" />

# RESULT:
The Commands are executed successfully.
