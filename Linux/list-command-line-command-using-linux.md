## List commandline common in Linux - Command-Line Interface CLI


## Working OS:
cat /etc/os-release  	: checking version of OS
cat /proc/cpuinfo       :
cat /etc/hosts		:
df -m			: get a report on the system's disk space
du -h			: Disk Usage check how much space a file or a directory takes
uname			: Unix Name, print detailed information about Linux System...
ps			: process statuses - a snapshot of all running processes.
ps aux			: a - all running process
			: u - information of memory, cpu
			: x - option lists all
top			: used to discover resource-hungry processes
htop			:
history			: to review the commands you've entered before. 
man tail 		: show the manual instr
useradd	manhkm		: add new person named manhkm
passwd 123456		: add password type


## Working directory
pwd			: find out the path of the current working directory
ls -al			: list add file, directory in current working directory
cd .. 			: back to 1 level
cd ../../		: back to 2 level
clear 			: clear data in screen desktop
exit			: exit windows
history			: check history of command line
mkdir music		: to make a new directory
mkdir music/newfile	:
mkdir -p music/2022/newfile: create the new "2022" file
rmdir			: to delete a directory | only delete empty directory
rm 			: to delete directory and the contents within them.
rm -r			:
tar -cvf data01.tar /root/study/manhkm/data/music/2022/newfile: zip file
zip			: 
unzip			:



## Working file
cat file_name		: reading/show content in file_name
gunzip			: zip file
cat file_name		:
cat > file_name		: create a new file
cat filename1 filename2 > filename3	: join two file 1, 2 and stores the output of them in a new file 3
cp picture.jpg /home/username/picture	: copy files from the current directory to a different directory
mv file.txt /home/username/document 	: move file, can also be used to rename files.
mv oldname.txt newname.txt		: rename file
touch /home/username/document/data.txt	: to create a blank new file
locate -i schoole*note	: search for any file that containt word "school" and "note", whether it is uppercase or lowercase
find /home/ -name notes.txt		: search for a file called notes.txt within the "home" directory and subdirectories
find . -name notes.txt 			: to find files in the current directory use
/ -type d -name note.txt		: to look for directories user
grep blue notepad.txt	: search for the word "blue" in the notepad file.
head -n 5 filename.txt	: to view the first lines of any text file
tail -n 10 filename.txt	: will display the last ten line of a text file
diff file1.txt file2.txt		: to compares the contents of 2 file.
echo Hello, data >> name.txt		: to move some data into a file





## Working networking
telnet ip port 		: checking connection to ip+port
ssh root@10.38.31.21	:
top && q		:
netstat -anp |grep 9001	: check port in module
ping your_ip		: to check connectivity status to server
hostname		: show name of your host/network
hostname -i		: display the IP address of your network



## Working grant role
su username 		: switch to username
ps -r			:
ps -ef | grep content	: show info grep content
pwdx 23473		: check path of PID
sudo			:
chmod OWNER[:group] Files : to change the read, write, execute permission of file or directories
ps ux			: show PID running in OS
kill [signal option] PID: to terminate manually


## Working TCP/IP
### Connection FTP Server:
which tcpdump		: check path of tcpdump
sudo dnf install -y tcpdump	: install tcpdump in CentOS or Red Hat Enterprise Linux
tcpdump --list-interfaces	: to see which interfaces are available for capture
sudo tcpdump -D
sudo tcpdump --interface any	:
sudo tcpdump -i any -c 5	:



ftp ip port		:



## Reference document

1. CLI tutorial: https://www.hostinger.com/tutorials/what-is-cli
2. Linux command tutorial: https://www.hostinger.com/tutorials/linux-commands





