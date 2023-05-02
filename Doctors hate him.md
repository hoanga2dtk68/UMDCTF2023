# Forensics
Tiến hành extract file chm author cho để lấy flag có thể extract bằng các công cụ như 7z, ...
xem qua các file thì đa số là file nhị phân có ảnh cần xem xét và file .html 
mở trên web thì không có gì đặc biệt
![image](https://user-images.githubusercontent.com/110059218/235687875-491d9521-06f4-49b1-bf6b-7e30314a9029.png)
vào source code để đọc

![image](https://user-images.githubusercontent.com/110059218/235688339-d314c100-9cd7-4099-9d77-0ab9c1733e6e.png)
thì có 2 base64 được mã hóa 1 cái được thực thi ngầm qua powershell để cưỡng chế cài explorer.exe và thực thi mã độc

![image](https://user-images.githubusercontent.com/110059218/235688261-6f4b6015-c624-43fc-9d6d-8b1ccb6668bf.png)
decode lấy được part 1: UMDCTF{1997_called_

![image](https://user-images.githubusercontent.com/110059218/235688548-dd0eea2b-75a9-49c3-91ea-2f1dbc07d361.png)
phần base64 sau decode ra thì có thể được địa chỉ để tải trình duyệt và thực thi
![image](https://user-images.githubusercontent.com/110059218/235688793-41b4d6a3-a079-44fb-9d99-467f17afb53f.png)
khi truy cập web thì có 2 file file sau có thể chính là một phần có flag và mở ra là base64 sau decode là part3 của flag
![image](https://user-images.githubusercontent.com/110059218/235689083-c94e9866-942f-4bab-988c-2ca7a3c6f258.png)
cho file explorer.exe lên virustotal thì 
![image](https://user-images.githubusercontent.com/110059218/235690189-1af267e6-384b-48e6-99d1-179add9d4e68.png)
part 2 rot13 đoạn cuối base64 

![image](https://user-images.githubusercontent.com/110059218/235690429-4c9cad08-d1c7-4e5c-9882-ef48148a7d5d.png)
![image](https://user-images.githubusercontent.com/110059218/235690534-c22659ff-cf72-434a-9a42-9cb2be3bfbce.png)
bingo: UMDCTF{1997_called_they_want_their_malware_back_bozo}
