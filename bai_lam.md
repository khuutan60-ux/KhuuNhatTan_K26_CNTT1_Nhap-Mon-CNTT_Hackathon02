# BÀI LÀM – HACKATHON 02

- **Mã đề:** 03
- **Họ tên:**Khưu Nhật Tân
- **Lớp:**CNTT1
- **Link repository:**
- **Hệ điều hành (Windows/macOS):**Windows

## 4.2. Thao tác máy tính cơ bản bằng CLI

### Các lệnh đã chạy

```shell
# Ghi lần lượt các lệnh đã chạy, mỗi lệnh một dòng
PS D:\> cd D:\starter-kit\karaoke-website
PS D:\starter-kit\karaoke-website> ls -Force
PS D:\starter-kit\karaoke-website> mv .\Ghi_Chu_Ky_Thuat.txt docs
PS D:\starter-kit\karaoke-website> mkdir backup
PS D:\starter-kit\karaoke-website> cp .\data\Dat_Phong_Thang_3.xlsx backup
PS D:\starter-kit\karaoke-website> rm *.tmp
PS D:\starter-kit\karaoke-website> cd .\logs\
PS D:\starter-kit\karaoke-website\logs> ls
PS D:\starter-kit\karaoke-website\logs> cd ..
```

### Kết quả liệt kê toàn bộ dự án (Windows: Get-ChildItem -Recurse -Force; macOS: ls -aR)

```text
PS D:\> cd D:\starter-kit\karaoke-website
PS D:\starter-kit\karaoke-website> ls -Force


    Directory: D:\starter-kit\karaoke-website


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        11/11/2026   8:02 AM                data
d-----        11/11/2026   7:59 AM                docs
d-----        11/11/2026   7:59 AM                evidence
d-----        11/11/2026   8:02 AM                logs
d-----        11/11/2026   8:02 AM                web
-a----         11/3/2026   7:07 AM             70 .env
-a----         11/3/2026   7:07 AM           2410 bai_lam.md
-a----         11/3/2026   7:07 AM            163 Ghi_Chu_Ky_Thuat.txt
-a----         11/3/2026   7:07 AM             22 temp_303.tmp


PS D:\starter-kit\karaoke-website> mv .\Ghi_Chu_Ky_Thuat.txt docs
PS D:\starter-kit\karaoke-website> mkdir backup


    Directory: D:\starter-kit\karaoke-website


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
d-----        11/11/2026   8:06 AM                backup


PS D:\starter-kit\karaoke-website> cp .\data\Dat_Phong_Thang_3.xlsx backup
PS D:\starter-kit\karaoke-website> rm *.tmp
PS D:\starter-kit\karaoke-website> cd .\logs\
PS D:\starter-kit\karaoke-website\logs> ls


    Directory: D:\starter-kit\karaoke-website\logs


Mode                 LastWriteTime         Length Name
----                 -------------         ------ ----
-a----         11/3/2026   7:07 AM            994 Booking.log


PS D:\starter-kit\karaoke-website\logs> cd ..

```

## 4.3. Lọc log truy cập website

### a) Lệnh lọc các dòng status=500

```shell
PS D:\starter-kit\karaoke-website> Select-String "status=500" .\logs\Booking.log >.\logs\loi_500.txt

```

### 2 dòng đầu tiên trong logs/loi_500.txt

```text
logs\Booking.log:5:2026-03-28 08:13:01 POST /api/thanh-toan status=500
logs\Booking.log:6:2026-03-28 08:17:12 POST /api/thanh-toan status=500

```

### b) Lệnh đếm số dòng status=404 và kết quả

```shell
PS D:\starter-kit\karaoke-website> ( Get-Content .\logs\Booking.log | Select-String "status=404").count

```

```text
4

```

## 4.4. Chạy script tong_hop (.ps1 hoặc .sh)

### Lệnh chạy (Windows: nếu dùng Phụ lục 2 thì ghi cả 2 lệnh)

```shell
# Ghi lệnh vào đây (xoá dòng này)

```

### Nội dung file logs/tong_hop.txt

```text
(Dán nội dung file vào đây – xoá dòng này)

```

## 4.5. README.md và bảo vệ thông tin bí mật

> README.md, .gitignore và .env.example được chấm trực tiếp trên file ở gốc dự án. Đánh dấu `[x]` vào các mục đã làm để tự kiểm tra.

- [ ] README.md: Heading 1, mô tả có **in đậm** và *in nghiêng*, bảng, code block, task list, blockquote
- [ ] .gitignore có dòng `.env` (tên file đúng, không có đuôi .txt)
- [ ] .env.example có đủ tên biến, giá trị để trống (tên file đúng, không có đuôi .txt)

## 4.6. Kiểm tra trang web bằng DevTools (F12) và báo cáo lỗi

### Bảng lỗi

| STT | Tab DevTools phát hiện lỗi | Tên file hoặc thông báo lỗi | Cách khắc phục |
| --- | --- | --- | --- |
| 1 |  |  |  |
| 2 |  |  |  |

> Ảnh chụp màn hình lưu trong thư mục `evidence/` (network.png, console.png).

### Báo cáo lỗi gửi trưởng nhóm

- **Context:** 
- **Expected:** 
- **Actual:** 
- **Log:** 

### Câu tìm kiếm Google

```text
(Ghi câu tìm kiếm vào đây – xoá dòng này)

```

## 4.7. Excel

> Phần Excel được chấm trực tiếp trên file `data/dat_phong_thang_3.xlsx`, không cần ghi vào đây.
