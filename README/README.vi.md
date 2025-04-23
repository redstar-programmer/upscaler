# Redstar Upscaler
Video mạnh mẽ Công cụ nâng cấp FFMPEG, Real-Esrgan, FlowFrames-Now hỗ trợ ** UI đa ngôn ngữ **!

## Cài đặt ngôn ngữ / ngôn ngữ
[Hàn Quốc] (readme/readme.md) | [Tiếng Anh] (Readme/Readme.en.MD) | [日本語] (readme/readme.ja.md) | [中文] (readme/readme.zh.md) |
[Français] (readme/readme.fr.md) | [Deutsch] (readme/readme.de.md) | [Español] (readme/readme.es.md) | [Bồ Đào Nha] (readme/readme.pt.md) |
[Р р [Ý] (Readme/readme.it.md) | [Tiếng việt] (readme/readme.vi.md) | [Bahasa Indonesia] (Readme/readme.id.md) |
[ภ ไทย ไทย] (readme/readme.th.md) | [ال] (readme/readme.ar.md)

<p align = "centre">
  Nó
</p>

<p align = "centre">
  <strong> ffmpeg, realesrgan, công cụ nâng cấp video dựa trên flowframes </strong> <br>
  <em> Cơ sở GUI mới nhất, cài đặt đặt trước, hỗ trợ xử lý nhiều tệp </em>
</p>

---

Tải xuống: [Phát hành]

##

Bạn có muốn thích dự án này hoặc phát triển hỗ trợ?  
Giúp một tính năng tốt hơn và cập nhật ổn định với một tài trợ nhỏ!  

-<img src = "https://img.shields.io/badge/donate-paypal-blue.svg?logo=paypal" height = "20"/> <br> ** paypal **: [https:  
-<img src = "https://img.shields.io/badge/sponsor-gigub20sorsors-f69b4?logo=githubsors


> Chi phí máy chủ, thời gian phát triển và một tách cà phê là một lực lượng lớn. Cảm ơn!

## Bảng nội dung

- [👋 Giới thiệu] (#Intringuction)  
-[Cài đặt và chuẩn bị] (#Cài đặt và chuẩn bị)  
- [🔧 Chức năng chính] (#Chức năng chính)  
-  
-[Mô tả chi tiết] (#Chi tiết-Chức năng-Description)  
- [🙏 Cảm ơn] (#Cảm ơn cảm ơn)  
- [📜 Lịch sử] (#History)

## Giới thiệu
** Redstar Upscaler ** là một công cụ GUI dựa trên Python tự động nâng cấp video lên độ phân giải cao bằng cách sử dụng `ffmpeg`, 'real-esrgan' và 'flowFrames'.

-THER FRAME VIDEO → Tăng cường → Kết hợp video cùng một lúc
-Support cho các mô hình Realesrgan khác nhau
-Optional thông qua các flowframes
-Audio Codec Extraction và xử lý
-Ta làm việc trên vị trí ban đầu hoặc đường dẫn được chỉ định

> Được phát triển và thử nghiệm trong môi trường Windows.

Dưới đây được kết nối với YouTube bằng cách nhấp vào màn hình sử dụng đơn giản. <br>
[! [Xem video trình diễn] (https://img.youtube.com/vi/g-jtwrws3co/0.jpg)] (https://youtu.be/g-jtwrws3co "

## Cài đặt và chuẩn bị

1. Việc cài đặt công cụ bên ngoài và xác nhận vị trí sau đây (tuy nhiên, tệp phân phối chứa các tệp cài đặt FFMPEG, Real-Esrgan và FlowFrames (xem các chương trình trong đường dẫn))
   - [ffmpeg] (https://www.ffmpe.org/doad.html)
   -[Real-Esrgan] (https://github.com/xinntao/real-esrgan
   - [FlowFrames] (https://github.com/n00mkrad/flowframes) *(chọn) * *
2. Chạy Upscaler.exe của Readstar sau khi giải nén
3. Trong trường hợp của các khung hình lưu lượng, các mô hình được tải theo môi trường người dùng có thể khác nhau, vì vậy hãy chắc chắn chạy các flowframes và sau đó <br> Nội suy AI và Redstar Upscaler tài nguyên UPSCaler/FlowFrames_Models.ini phải khớp. <br> Các mô hình không tải được ghi nhận để được nhận xét thông qua màn hình # và chắc chắn kiểm tra xem thứ tự mô hình của cửa sổ cài đặt của UPSCaler Redstar có khớp với thứ tự mô hình của <br> flowframes hay không.

## chức năng chính

!! [Hình ảnh] (https://github.com/user-attachments/assets/93DC232E-8742-4AE3-935-9395C26A61F4)
-Video nhiều lựa chọn và công việc tuần tự
-Add kéo/thả/thả
-✅ có nên chạy các chương trình lớn hay không và chọn lựa chọn trực tiếp
-Chế độ tiết kiệm
-Cultual Hỗ trợ (15 ngôn ngữ)
<br> <br>
!! [Hình ảnh] (https://github.com/user-attachments/assets/3341f4ca-af20-4647-93d0-4841466757)
-Save đặt trước và ứng dụng tự động
-Phình phát hiện của Codec âm thanh và cài đặt SetRate
-Tôi phát hiện và lựa chọn các mô hình Realesrgan
-Ffmpeg, real-esrgan, flowframes chi tiết
Cài đặt tùy chọn -Change theo phiên bản FlowFrames <br>
<br> <br>
!! [Hình ảnh] (https://github.com/user-attachments/assets/25D60D82-53A2-4064-bbef-d439d3d6)
-UpsCale Xác nhận thứ tự thực hiện (có thể được sao chép và thực thi riêng biệt với CMD)
<br> <br>
!! [Hình ảnh] (https://github.com/user-attachments/assets/2fd69862-d038-401d-a9a6-83dc84c769f0)
-Monitor tiến bộ tổng thể của công việc cao cấp
-UpsCale Xác nhận ghi nhật ký (tệp nhật ký được tạo dưới dạng ngày trong thư mục nhật ký trong thư mục thực)
-N
-Các hoạt động sau khi hoàn thành <br>
<br> <br>
## Cách sử dụng (Bắt đầu nhanh)

1. Thêm tệp video (MP4, MKV, AVI, MOV, FLV, WMV, MPG, WebM, 3GP, OGV)
2. Kiểm tra vị trí công việc hoặc kiểm tra "Sử dụng đường dẫn tệp gốc"
3. Nhấp vào nút "Cài đặt" trong video được thêm
4.
5. Nhấp vào chỉ áp dụng cho toàn bộ tệp / chọn tệp
4. Nhấp vào nút Xác nhận nhiệm vụ
7. Nhấp vào nút Bắt đầu sau khi kiểm tra lệnh để chạy

> Kết quả công việc được tạo trong thư mục được chọn bởi hai hình ảnh được nâng cấp và hai tệp video được nội suy khung.
> Tệp hoàn thành được lưu dưới dạng tên tệp với tiền tố [Redstar].
---

## Mô tả chi tiết

| Mục | Mô tả |
| ------ | ------ |
| ** Cài đặt đường dẫn nhiệm vụ ** | Cung cấp đường dẫn mặc định hoặc tùy chọn "Sử dụng đường dẫn tệp gốc" |
| ** Hỗ trợ định dạng video ** | MP4, MKV, AVI, MOV, FLV, WMV, MPG, WebM, 3GP, OGV, v.v.
| ** Mô hình cao cấp ** | Realesr-AnimeVideov3, Realesr-General, 4xplus, v.v.
| ** Xử lý âm thanh ** | Hỗ trợ mã hóa định dạng khác nhau như 'AAC', 'MP3' và 'FLAC' |
| ** Liên kết FlowFrames ** | Đặt nội suy (FPS × 2, × 4, × 8) |
| ** Chế độ tiết kiệm đĩa ** | Chức năng xóa tự động hình ảnh trung gian được cung cấp |

## 🙏 Lễ Tạ ơn

-RealSrgan bởi [Xinnntao] (https://github.com/xinntao/real-esrgan)
-FlowFrames bởi [N00MKRAD] (https://github.com/n00mkrad/flowframes)
-Nếu bạn muốn tham gia vào dự án này hoặc đề xuất một chức năng, vui lòng để lại ý kiến ​​về [các vấn đề] (https://github.com/redstar-javscraper/rredstar_upscaler/issues).

# Lịch sử

v 1.1.0
 >. Cấu hình menu (mở tệp, đóng, cài đặt nhật ký, cài đặt ngôn ngữ)
 > 2. Thêm nhiều cài đặt ngôn ngữ (Ngôn ngữ có sẵn: tiếng Hàn, tiếng Anh, 日本語, 中文, Français, Deutsch, Español, Bồ Đào Nha, рс
 3. Thông điệp và một số thay đổi mã theo cài đặt ngôn ngữ
 > 4. Thay đổi một số cấu hình UI
 >. Ffmpeg, real-esrgan, flowframes mỗi thông tin phiên bản (màn hình chính)
 > 6. FlowFrames 1.41.0 Phản hồi (phiên bản hiện tại 1.41.0 có sự cố lệnh CMD, do đó, chỉ có thể sử dụng 1.40.0 và 1.36.0)
 > Giải quyết vấn đề ở chỗ mục mô hình AI được hiển thị dưới dạng chữ thường
 8. Tùy chọn FFMPEG (pixel, codec video)
 > 9. Củng cố kiểm tra CUDA cho người dùng PCS -có thể được sử dụng và kiểm tra loại GPU (màn hình chính)

v 1.0.0
 >.
 >. Ui thay đổi
 > 3. Tăng phạm vi video/âm thanh có thể xử lý
 > 4. Thêm chế độ lưu đĩa
 > Phân phối bao gồm các chương trình chính

v 0.1,92
 >. FlowFrames Vấn đề thất bại nội suy bằng cách trùng lặp đầu vào trong hộp combo mô hình AI khi thay đổi con đường
 > 2. Thêm trạng thái lựa chọn của hộp kết hợp cho công việc nội suy

v 0.1,91
 >.
 > 2. Điều chỉnh tệp phân phối

v 0.1.9
 >. Ứng dụng thay đổi mô hình flowframes
 >. FlowFrames 1.36.0 Mô hình mới, triển khai mô hình 1.40.0
 3. Không còn sự thất bại của lệnh flowframes nữa
 > 4. Bạn có thể thêm các tệp với kéo/thả
 > Giải quyết vấn đề không được áp dụng

v 0.1.8
 >.
 2. Nếu FlowFrames được cài đặt trong đường dẫn mặc định (ví dụ C: \ Users \ Quản trị viên
 3. Khi thêm nhiều tệp 
 > 4. Sau khi thêm nhiều tệp,

v 0.1.7
 >. Thay đổi kích thước chương trình
 2. Giải quyết vấn đề lỗi khi làm việc với một tệp không có giọng nói
 > 3. Thay đổi toàn bộ cấu hình UI (được cấu hình lại để phù hợp với thay đổi kích thước)

v 0.1.6
 >.
 >. Giải quyết vấn đề mà thông tin phiên bản không được xem là phiên bản mới trong tiêu đề chương trình.
 > Giải quyết vấn đề trong đó các tệp config.ini được lưu trữ trong các đường dẫn khác
 > 4. Khi thay đổi hệ thống thoát nước cao cấp Realesrgan, hộp combo mô hình cao cấp cũng được thay đổi cùng nhau
 > 5. Thêm chức năng kiểm tra cập nhật
 > 6. Một số sửa đổi logic
 > 7. Độ phân giải và FPS
 > 8. Sửa đổi người dùng (trước đây) (phải được nhập dưới dạng 1024x768)

v 0.1,5
 >.
 2.
 3. Thêm một số video về hộp kết hợp "FPS tính toán" để ngăn chặn trường hợp được tính là FPS sai khi tính toán FPS của một số video.
        -> R_FRAME_RATE / AVG_FRAME_RATE có thể được chọn và mặc định được tính bằng R_FRAME_RATE
 > 4. Khi chọn tệp video, tiến trình của thông tin video 
 > 5. Sau khi tệp được khởi động, thay đổi để mở thư mục được chọn cuối cùng theo mặc định khi chọn lại tệp.

v 0.1.4
 >. Config.ini thay đổi phương thức đọc tệp
 > 2. Thay đổi thông tin video từ Python AV thành FFMPEG
 > 3. Thêm chức năng Windows End khi làm việc
 > 4. Trong danh sách công việc, toàn bộ tên tệp được hiển thị dưới dạng công cụ
 >. Trong danh sách công việc, mỗi độ phân giải tệp (trước) / độ phân giải (sau) / fps (trước) / fps (bài đăng) ký hiệu
 > 6. Loại bỏ hộp đầu vào FPS (loại bỏ do mỗi ký hiệu tệp)
 > 7. Loại bỏ kích thước dự báo FPS đầu ra (loại bỏ do mỗi tệp cho mỗi tệp)
 > 8. Trạng thái tiến trình được viết là hai proessbar bằng toàn bộ tệp/công việc

v 0.1.3
 > 1. Khắc phục lỗi tính toán FPS FPS với một số thông tin FPS khi nhập tệp

v 0.1.2
 >. Thay đổi cấu hình UI   
 > 2. Thay đổi logic bên trong  
 > Giải quyết vấn đề không được thực thi khi chọn hai mô hình bên dưới giữa các mô hình Realesrgan  
 > 4. Thay đổi cách sử dụng mô hình Realesrgan   
 > -> Sao chép một tệp mô hình mới (*.Param) vào thư mục mô hình trong thư mục cài đặt Realesrgan có sẵn.  
 >.  
 > 6. Mã di chuyển tệp config.ini  
 > 7. Hình ảnh phân hủy ffmpeg aac-> flac  
 > 8. Sửa đổi lỗi khác

v 0.1.1
 >. Viết ban đầu, ffmepg, realesrgan và flowframes.