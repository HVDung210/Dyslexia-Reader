# README - Ứng dụng Dyslexia-Reader
## Giới thiệu
Đây là repo cho bài tập lớn môn <b>Các vấn đề hiện đại trong KHMT</b><br>
Mã môn học:  <b>INT3011E 5</b><br>
Nhóm: 12. Chủ đề: <b>Xây dựng ứng dụng Dyslexia-Reader - Ứng dụng hỗ trợ đọc sách cho người khó đọc</b>

<b>Thành viên</b>:
<ul>
  <li>Hoàng Văn Dũng - MSV: 22028188</li>
  <li>Nguyễn Đức Duy - MSV: 22028215</li>
  <li>Lê Minh Dương - MSV: 22028283</li>
  <li>Nguyễn Văn Hưng - MSV: 22028118</li>
</ul>

 ## Mục tiêu:
<ul>
  <li>Cung cấp giải pháp hỗ trợ cho người mắc hội chứng khó đọc</li>
  <li>Cải thiện khả năng tiếp cận đọc thông qua công nghệ</li>
  <li>Tạo ra trải nghiệm đọc thân thiện với người dùng</li>
</ul>

## Tổng quan

Dyslexia Reader là một ứng dụng di động Android được thiết kế để hỗ trợ người mắc chứng khó đọc, cung cấp trải nghiệm đọc sách điện tử được tối ưu hóa. Ứng dụng cho phép tải lên hoặc quét tài liệu cá nhân, quản lý thư viện sách điện tử và cung cấp các tính năng đọc chuyên biệt để tăng khả năng tiếp cận cho người gặp khó khăn trong việc đọc. Các tính năng chính bao gồm tùy chỉnh hiển thị văn bản, làm nổi bật từ, tra cứu từ với hình ảnh minh họa do AI tạo và hỗ trợ nhiều định dạng sách điện tử (PDF, EPUB, DOCX, JPEG, PNG, JPG).

## Tính năng

1.  **Tải lên và Quét Tài liệu**

    *   **Tải lên:** Người dùng có thể tải sách điện tử ở các định dạng như PDF, DOCX, EPUB, PNG, JPG và JPEG.
    *   **Quét:** Chụp tài liệu vật lý bằng camera thiết bị, với nội dung được trích xuất bằng Google ML Kit.
    *   **Lưu trữ:** Tất cả tệp được lưu trên Firebase để truy cập liền mạch trên nhiều thiết bị.

2.  **Quản lý Thư viện Sách Điện tử**

    *   Xem, sắp xếp và quản lý sách điện tử với thông tin chi tiết như tiêu đề, ảnh bìa, tác giả và tiến độ đọc.
    *   Sắp xếp sách theo danh mục: "Your Books", "Favourites", "Reading" và "Complete".
    *   Cập nhật thời gian thực cho các thao tác như thêm, xóa hoặc đánh dấu sách yêu thích, đồng bộ qua Firebase.

3.  **Hỗ trợ Đọc Chuyên biệt**

    *   **Tùy chỉnh Hiển thị:** Điều chỉnh kiểu chữ, kích thước, khoảng cách, màu nền và màu chữ để giảm căng thẳng khi đọc.
    *   **Làm nổi bật Từ:** Làm nổi bật từ, dòng hoặc vùng văn bản trong khi đọc để tăng tập trung, kích hoạt bằng tương tác chạm.
    *   **Tra cứu Từ:** Nhấn đúp vào từ để xem cách phát âm (qua Google TTS), định nghĩa và hình ảnh minh họa do AI tạo (sử dụng Llama qua GroqCloud và pollinations.ai).
    *   **Theo dõi Tiến độ Đọc:** Đo tốc độ và thời gian đọc để cung cấp phản hồi về sự tiến bộ.
    *   **Định dạng Dễ tiếp cận:** Làm nổi bật ký tự khó đọc và hỗ trợ chuyển văn bản thành giọng nói để hiểu rõ hơn.

## Đối tượng Người dùng

Ứng dụng hướng đến người mắc chứng khó đọc, cung cấp trải nghiệm đọc tương tự các ứng dụng đọc sách phổ biến như Kindle hoặc Apple Books. Mục tiêu là giúp người khó đọc có trải nghiệm đọc thoải mái, bình đẳng và phong phú.

## Công nghệ Sử dụng

*   Android SDK: Phát triển giao diện, điều hướng và tương tác người dùng.
*   Firebase: Lưu trữ đám mây cho sách điện tử và đồng bộ dữ liệu người dùng.
*   Thư viện Trích xuất Văn bản:
    *   Mammoth (Zwobble) cho DOCX.
    *   iTextPDF (Apryse) cho PDF.
    *   Epublib (Paul Siegmann) cho EPUB.
    *   Google ML Kit cho trích xuất văn bản từ hình ảnh (PNG, JPG, JPEG).
*   Tích hợp AI:
    *   Llama (qua GroqCloud) cho tạo văn bản.
    *   pollinations.ai cho hình ảnh minh họa do AI tạo.
    *   Google Text-to-Speech (TTS) cho phát âm từ.
*   Backend: Dịch vụ web được lưu trữ trên Render để tích hợp mô hình AI.

## Cài đặt

**Cách 1: Cài đặt qua APK**

1.  Tải APK từ: [[Google Drive](your_google_drive_link_here).](https://drive.google.com/file/d/1H-aEMtGvH9yIoePISlO3nxlHcecEQJtF/view)
2.  Cài đặt APK trên thiết bị Android.
3.  Khởi chạy ứng dụng.

**Cách 2: Cài đặt từ Mã nguồn**

1.  Cài đặt Android Studio và Android SDK.
2.  Tải mã nguồn từ: [[GitHub](your_github_repository_link_here).](https://github.com/HVDung210/Dyslexia-Reader)
3.  Giải nén và mở thư mục dự án trong Android Studio.
4.  Kết nối thiết bị Android qua USB Debugger.
5.  Chọn thiết bị Android đã kết nối trong Android Studio.
6.  Nhấn nút "Run" để xây dựng và cài đặt ứng dụng.

## Hướng dẫn Sử dụng

*   **Đăng nhập:** Đăng nhập để truy cập thư viện cá nhân.
*   **Tải/Quét Tài liệu:** Vào trang "Library" để tải sách điện tử hoặc quét tài liệu vật lý.
*   **Quản lý Thư viện:** Xem, sắp xếp hoặc xóa sách trong các mục "Your Books", "Favourites", "Reading" hoặc "Complete".
*   **Đọc Sách:** Chọn sách, tùy chỉnh cài đặt hiển thị và sử dụng các tính năng như làm nổi bật từ hoặc tra cứu từ.
*   **Khám phá Gợi ý:** Xem gợi ý sách trên "Main Menu" dựa trên lịch sử đọc.
