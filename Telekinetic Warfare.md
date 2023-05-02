# Stego
Đầu bài cho một file gif đầu tiên thấy dung lượn rất lớn chứng tỏ được hợp thành từ rất nhiều ảnh, sau khi dùng tool online quét được ảnh đầu tiên thì quét qr nhận được đoạn base64 decode ra phần đầu của header là header của pdf
Sau đấy dùng kha kha tool không tách thành công thì dùng tool ffmpeg tách ra được khoảng 14k ảnh qr sau khi quét qua vài ảnh thì có thể thấy ghép lại sẽ ra được một file pdf
** ffmpeg với -i là input
![image](https://user-images.githubusercontent.com/110059218/235676923-edf833ab-b11f-45ea-a348-14d17106e701.png)
![image](https://user-images.githubusercontent.com/110059218/235676968-51776d11-4f23-4213-b839-e84514202103.png)
** ảnh decode ảnh được tách đầu tiên
![image](https://user-images.githubusercontent.com/110059218/235677500-17174f21-4903-457e-9c23-065125dbd455.png)
Sau đó code để giải quyết việc quét 14k ảnh ra base64 decode và để dạng đuôi .pdf để nhận flag
![image](https://user-images.githubusercontent.com/110059218/235677811-65a21f66-dee0-41a2-974a-42fa0ce2b3c8.png)
chạy file python
![image](https://user-images.githubusercontent.com/110059218/235678769-c10a149f-5aff-4de9-85cc-8929700090b1.png)
decode base64 nhận flag
![image](https://user-images.githubusercontent.com/110059218/235679136-f455dbfc-c6c0-4aa4-bbd1-f25aad1edc01.png)
bingo: UMDCTF{wh0_n33d5_k1net1c_w4rfar3_anyw4ys}
