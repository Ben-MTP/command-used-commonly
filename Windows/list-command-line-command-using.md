# Danh sách các command line thường sử dụng trên windows:

## Làm việc với thư mục:
dir					: hiển thị các thư mục, file trong đường dẫn path.
tree /f				: hiển thị các file, thư mục dưới dạng tree
mkdir name_dir 		: tạo thư mục mới name_directory
rmdir name_dir      : xóa directories/folders
rd name_dir			: giống với mrdir name_dir
rmdir /s name_dir   : thực hiện xóa directory chứa toàn bộ các thư mục con/file trong đó.



## Làm việc với file:
type your_name.txt			: đọc file your_name.txt
echo your_data > sample.txt : ghi dữ liệu vào file sample.txt
del "your_name.txt"			: xóa file your_name.txt
del /f "your_name.txt"		: dựng cờ buộc xóa file này
notepad name_f.txt  		: đọc name_f.txt với GUI notepad


## Kiểm tra thông tin mạng
netsh wlan show interfaces		: thông tin về mạng wifi đang sử dụng
netstat -a						: chỉ ra các connection hiện tại và protocol, source, destination address
netstat -b  					: chỉ ra executable involved trong mỗi connection or listening port
netstat /?						: chỉ ra tất cả các option với dòng lệnh tương ứng.
