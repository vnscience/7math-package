# 7Math - Trợ lý soạn thảo đề thi và giáo án Toán học

7Math là một ứng dụng web tĩnh hỗ trợ giáo viên và giảng viên Toán học tại Việt Nam biên soạn đề thi trắc nghiệm, đề tự luận và giáo án. Ứng dụng tập trung tối ưu hóa trải nghiệm người dùng không chuyên (low-tech), cho phép tạo nhanh các tài liệu Toán học theo chuẩn cấu trúc của Bộ Giáo dục mà không đòi hỏi người dùng phải ghi nhớ mã nguồn LaTeX phức tạp.

## Tính năng nổi bật

### 1. Trình dựng công thức trực quan (Word-Style)

Hệ thống cung cấp giao diện nhập liệu mô phỏng không gian vị trí thực tế tương tự như công cụ Equation tích hợp sẵn trong Microsoft Word:

- Phân số: Ô nhập tử số nằm phía trên và mẫu số nằm phía dưới, ngăn cách bởi đường kẻ ngang trực quan.

- Căn thức: Khung nhập liệu nằm trọn dưới ký hiệu căn bậc hai.

- Lũy thừa: Ô nhập số mũ thu nhỏ được xếp cao hơn ở góc trên bên phải của cơ số.

- Lôgarit: Ô cơ số nằm dưới chân và ô biểu thức nằm ngang dòng trong dấu đóng mở ngoặc.

- Giới hạn (Limit): Phân bổ ô nhập biến số tiến về giá trị bên dưới ký tự giới hạn và biểu thức phía sau.

- Tích phân và Tổng Sigma: Có sẵn các ô nhập cận trên, cận dưới và biểu thức tương ứng.

- Vectơ: Nhập trực tiếp tên vectơ dưới ký hiệu mũi tên định hướng nằm ngang dòng.

- Hệ phương trình và Ma trận: Cho phép điền các dòng phương trình song song tự động căn lề sau dấu ngoặc nhọn hoặc ngoặc vuông.

### 2. Trình tạo câu hỏi trắc nghiệm tự động

Giáo viên chỉ cần điền nội dung câu hỏi dạng văn bản thông thường, nhập 4 đáp án vào các ô A, B, C, D. Hệ thống sẽ tự động ghép thành câu hỏi trắc nghiệm hoàn chỉnh, căn lề thẳng hàng và tự động tăng số thứ tự câu tiếp theo (Câu 1, Câu 2, Câu 3...) để tối giản thao tác lặp lại.

### 3. Tối ưu hóa bản in PDF

Ứng dụng tích hợp cấu hình CSS Print chuyên biệt nhằm đảm bảo chất lượng xuất bản PDF qua trình duyệt:

Tự động ẩn toàn bộ thanh công cụ, menu và sidebar điều khiển khi kích hoạt chế độ in.

Phông chữ trang in tự động chuyển về định dạng Times New Roman tiêu chuẩn.

Khoảng cách giữa các câu hỏi và đoạn văn được tự động co nén gọn gàng (Compact Spacing) để tiết kiệm giấy in.

Tự động kiểm soát việc ngắt trang (Page-Break), ngăn việc cắt đôi một câu hỏi trắc nghiệm hoặc khối công thức phức tạp ở mép trang giấy.

### 4. Hệ thống lịch sử và các tiện ích tích hợp

- Hoàn tác và Làm lại (Undo / Redo): Lưu trữ lịch sử biên soạn lên tới 50 trạng thái gần nhất, hỗ trợ cả nút bấm trực quan và phím tắt hệ thống (Ctrl + Z, Ctrl + Y).

- Lưu nháp cục bộ: Tự động lưu nội dung soạn thảo vào bộ nhớ trình duyệt (LocalStorage) theo từng phiên làm việc của giáo viên để tránh mất dữ liệu khi tắt máy đột ngột.

- Chế độ sáng/tối: Hỗ trợ thay đổi giao diện làm việc giúp bảo vệ mắt khi làm việc ban đêm.

## Công nghệ sử dụng

- Frontend: HTML5, CSS3, Tailwind CSS.

- Bộ dựng công thức: MathJax v3 (TeX-to-CHTML) giúp hiển thị biểu thức toán học dạng vector sắc nét ngay trên trình duyệt mà không cần kết nối máy chủ.

- Hệ phông chữ: Inter (Giao diện điều khiển) và JetBrains Mono (Vùng nhập liệu mã nguồn).

## Hướng dẫn cài đặt và sử dụng

7Math là một ứng dụng web tĩnh đơn tệp (Single-File Web App), không yêu cầu cài đặt môi trường hay cấu hình máy chủ.

**Sử dụng ngoại tuyến (Offline) trên máy tính**

1. Tải tệp index.html về máy tính cá nhân.

2. Nhấp đúp chuột để mở tệp tin bằng trình duyệt web bất kỳ (Chrome, Edge, Safari, Firefox,...).

3. Biên soạn và xuất bản tài liệu trực tiếp mà không cần kết nối Internet.

## Hướng dẫn cấu hình in và xuất PDF

Để tệp tin PDF đạt tiêu chuẩn thẩm mỹ cao nhất, vui lòng thực hiện các bước sau khi chọn chức năng "Xuất PDF / In Đề":

1. Tại hộp thoại cấu hình in của hệ thống, chọn mục đích đến là **Lưu dưới dạng PDF** (Save as PDF).

2. Mở phần **Cài đặt khác **(More settings).

3. **Bắt buộc**: Bỏ chọn mục **Tiêu đề và chân trang** (Headers and footers) để loại bỏ các thông tin liên kết và ngày tháng không mong muốn của trình duyệt ở đầu và cuối trang.

4. Đảm bảo tỷ lệ căn lề (Margins) được đặt ở mức **Mặc định** (Default).

5. Xác nhận **Lưu** (Save) để tải về tệp PDF hoàn chỉnh.

## Đóng góp phát triển

Mọi ý kiến đóng góp nhằm cải tiến giao diện hoặc bổ sung thêm các mẫu toán học phổ thông mới đều được ghi nhận:

1. Fork dự án này.

2. Tạo nhánh tính năng mới (git checkout -b feature/NewFeature).

3. Commit các thay đổi (git commit -m 'Add NewFeature').

4. Push nhánh lên GitHub (git push origin feature/NewFeature).

5. Tạo một Pull Request mới.

## Giấy phép (License)

Dự án này được phát hành theo giấy phép MIT License. Thầy cô và các lập trình viên có thể tự do sao chép, chỉnh sửa và chia sẻ cho mục đích phi thương mại hoặc thương mại.
