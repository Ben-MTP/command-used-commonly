## List commandline common in Linux - Command-Line Interface CLI


## Working OS:
cat /etc/os-release  	: checking version of OS
cat /proc/cpuinfo       :
cat /etc/hosts			:
df -m					: get a report on the system's disk space
df -h 					: show info disk with %
du -h					: Disk Usage check how much space a file or a directory takes
uname					: Unix Name, print detailed information about Linux System...
ps						: process statuses - a snapshot of all running processes.
ps aux					: a - all running process
						: u - information of memory, cpu
						: x - option lists all
top						: used to discover resource-hungry processes
htop					:
history					: to review the commands you've entered before. 
man tail 				: show the manual instr
useradd	manhkm			: add new person named manhkm
passwd 123456			: add password type
who -a					: id -a hoặc whoami - kiểm tra người dùng
kill cửa sổ 

cat /proc/cpuinfo		: xem thông tin về CPU sảm xuất
cat /proc/meminfo		: xem thông tin về RAM sản xuất
free					: xem thông tin RAM
						: swap - bộ nhớ hoán đổi
df -h 					: xem HDD


## Pipe command:
pipes					: đầu ra của đằng trước được đưa vào đằng sau
command1 | command2 | ... commandN



## Chuyển hướng dữ liệu vào file:
ls -al | grep bash		: 
ls -al >> /tmp/test.log	: append file
ls -al > /tmp/test.log	: thêm mới file
ls -al | grep bash | wc -l > /tmp/test_manhkm2.log

stdout > file 			: lấy dữ liệu đầu ra chuẩn ghi vào file
stderr 2> file 			: lấy dữ liệu đầu ra lỗi ghi vào file
stdout + stderr &> file : lấy cả dữ liệu chuẩn + lỗi ghi vào file

md5sum -b .tcshrc		: 
locate content_check	: tìm thư mục hoặc file chứa nội dung trong content_check




## Working directory
pwd				: find out the path of the current working directory
ls -al			: list add file, directory in current working directory
cd .. 			: back to 1 level
cd ../../		: back to 2 level
clear, ctrl + l : clear data in screen desktop
exit			: exit windows
history			: check history of command line
				: execute command line with id in history: !ID
mkdir music		: to make a new directory
mkdir music/newfile	:
mkdir -p music/2022/newfile: create the new "2022" file
rmdir			: to delete a directory | only delete empty directory
rm 				: to delete directory and the contents within them.
rm -r			:
rm -rf 			: xóa tất mà không cần confirm
tar -cvf data01.tar /root/study/manhkm/data/music/2022/newfile: zip file
zip				: 
unzip			:
ctrl + r		: research command execute ago.

ls -l | wc -l	: count total file in directories




## Working file
cat file_name						: reading/show content in file_name
gunzip								: zip file
cat file_name						:
cat > file_name						: create a new file
cat filename1 filename2 > filename3	: join two file 1, 2 and stores the output of them in a new file 3
touch file_name						: create a new file

cp picture.jpg /home/username/picture	: copy files from the current directory to a different directory
cp /home/janet/clients/* /home/nick/customers
cp /root/abc.log .						: copy data đến thư mục hiện tại
cp -rv thu6 /tmp  						: copy data | -r con trỏ, v ??
mv file.txt /home/username/document 	: move file, can also be used to rename files.
mv oldname.txt newname.txt				: rename file or directory
touch /home/username/document/data.txt	: to create a blank new file
locate -i schoole*note			: search for any file that containt word "school" and "note", whether it is uppercase or lowercase
find /home/ -name notes.txt		: search for a file called notes.txt within the "home" directory and subdirectories
find . -name notes.txt 			: to find files in the current directory use
/ -type d -name note.txt		: to look for directories user
grep blue notepad.txt			: search for the word "blue" in the notepad file.
head -n 5 filename.txt			: to view the first lines of any text file
tail -n 10 filename.txt			: will display the last ten line of a text file
diff file1.txt file2.txt		: to compares the contents of 2 file.
echo Hello, data >> name.txt	: to move some data into a file

vi 			: soạn thảo trên file
	phím i -> insert
	phím d -> xóa dòng x2
	phím x -> mất kí tự
phím shif + :
	phím :wq! -> write and quit

## Read data in file:
cat file_name						: đọc nội dung của file
     + cat có thêm các tham số:
	 -n : đánh số mỗi dòng của output
	 -b : chỉ đánh dòng output không trống
	 -A : hiển thị ký hiệu xuống dòng
	 
more
less
tail -f /var/log/message.log		: chỉ in ra 10 dòng cuối cùng
     + giá trị -f dùng để đọc theo thời gian thực
	 
tail -100 -f /var/log/message.log 	: in ra 100 dòng cuối cùng
head -10 /var/log/...				: in cũng 100 dòng cuối cùng
phân biệt các tham số -f và -F		: khác nhau ở điều gì?
grep 'search_rules' *.*				: tìm kiếm thông tin trong file hoặc thư mục | grep <content> <thư mục/file>
----
tar --cvzf /tmp/xxx.tar.gz boot.log-	: tạo file nén
untar 

cmp 	: compare two files
cut		: 
echo	: ouput ra ngoài màn hình



## Working networking
telnet ip port 			: checking connection to ip+port
ctrl + ] 				: để thoát khỏi chế độ làm việc của Telnet
						: để logout khởi chế độ làm việc: close
ssh root@10.38.31.21	: truy cập ssh vào một server khác với username và ip tương ứng
top && q				: kiểm tra chỉ số tài nguyên của server
netstat -anp |grep 9001	: check port in module
ping your_ip			: to check connectivity status to server
hostname				: show name of your host/network
hostname -i				: display the IP address of your network
ip a					: xem ip v4
ip route				: xem default gateway
cat /etc/resolv.conf 	: xem DNS Server

## Switch User

su - 					: switch to user root
su - appgw 				: switch to user appgw


## Working grant role
su username 			: switch to username
ps -r					:
ps -ef | grep content	: show info grep content
pwdx 23473				: check path of PID
sudo					:
chmod OWNER[:group] Files 	: to change the read, write, execute permission of file or directories
ps aux						: show PID running in OS
kill [signal option] PID	: to terminate manually
change role cho file, thư mục:  chown -R appgw:neo /.......


## Grant role using character:
user owner -> u
group user -> g
others     -> o

role basic: read(r), write(w), execute(x)

chmod u+w abc.txt
chmod q+w abc.txt
chmod o+x abc.txt

chmod u-rwx, g-rwx, o-rwx abc.txt

## Grant role using number:
read = 4
write = 2
execute = 1
chmod 775 abc.txt
user 4 + 2 + 1
group 4 + 2 + 1
other 4 + 1


## Working TCP/IP
### Connection FTP Server:
which tcpdump				: check path of tcpdump
sudo dnf install -y tcpdump	: install tcpdump in CentOS or Red Hat Enterprise Linux
tcpdump --list-interfaces	: to see which interfaces are available for capture
sudo tcpdump -D
sudo tcpdump --interface any	:
sudo tcpdump -i any -c 5		:

### Catch package tcpdump

tcpdump -i any -s 65535 tcp port 5001 -w /tmp/trace_manhkm.pcap		: lấy gói tin tcpdump
Giai thich:
65535: do dai file
tcp port 5001: port can check ket noi, neu khong can thi bo
Thay xxx= port need check


ftp ip port		:

## Biến môi trường và các profile:
Biến môi trường là gì?
window: echo %Path%
	set XXX=VALUE_EVN
	echo %XXX%
	
linux: printenv
	
cat .bashrc

. .bash_profile: load danh sách các biến môi trường.

loading lên

## Tunnel SSH:
config tunnel trên các tool hay dùng
cấu hình filewal trên tool SecureCRT
ssh user@ip_server			: ssh đến một server thông qua một server khác


## Working crontab
crontab -l : check list crontab current in OS
crontab -e : config crontab in OS
tail -f /var/log/cron : kiểm tra log của các tiến trình đang chạy

scp -r  /app/appgw/adapter-db-cskh/libs appgw@ospadt02:/app/appgw/adapter-db-cskh/

câu lệnh chuyển copy thư mục của nó như sau: 
scp -r web/ appgw@10.3.19.3:/app/appgw/webadmin/

scp -r api/ appgw@10.3.19.3:/app/appgw/webadmin/

Hôm qua anh Khỉ hướng dẫn

đứng từ con 19.2 --> cd vào thư mục web --> copy sang 19.3


## Reference document

1. CLI tutorial: https://www.hostinger.com/tutorials/what-is-cli
2. Linux command tutorial: https://www.hostinger.com/tutorials/linux-commands





