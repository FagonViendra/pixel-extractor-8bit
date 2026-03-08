# Pixel Extractor 8-Bit PRO 🎨👾

Ứng dụng web siêu nhẹ giúp chuyển đổi, làm sạch và trích xuất ma trận pixel chuẩn 8-Bit từ các ảnh chụp, ảnh mờ hoặc ảnh AI bị vỡ nét (JPEG Artifacts/Anti-aliasing noise). 
Đặc biệt tối ưu để tạo mảng dữ liệu ảnh dùng cho HTML5 Canvas.

![Mô phỏng sử dụng](Screenshot%202026-03-08%20160708.png)

## Các tính năng chính (Version 3)

- **Auto Sync Real-Time:** Kéo thanh trượt đến đâu, hình và code cập nhật ngay đến đó. Không cần bấm nút!
- **Khử Nền Thông Minh (Noise Reduction):** Loại bỏ hoàn toàn các viền mờ xám xám/trắng nhạt bao quanh chủ thể (lỗi siêu phổ biến khi dùng ảnh AI).
- **Auto Bounding-Box:** Tự động cắt gọn khung ảnh, gom rác thừa, loại bỏ các ma trận khoảng trắng (Dấu cách) vô bổ giúp mảng (Array) xuất ra nhẹ và gọn gàng nhất.
- **Color Quantization (Bóp Bảng Màu):** Gom các điểm có màu nhang nhác giống nhau (Distance Tolerance theo thuật toán Euclidean) thành 1 màu chuẩn duy nhất. Cực kỳ hứu ích để ép 1 cái ảnh nát ngàn màu về đúng bảng 4-5 màu nguyên thủy.
- **Auto Code Gen:** Xuất thẳng ra mã JavaScript bao gồm `Bảng tham chiếu màu (Dictionary)` và `Ma Trận 2D (Array of Strings)` chuẩn chỉ. Chỉ việc copy/paste.

## Cài Đặt & Sử Dụng
- Đây là công cụ thuẩn HTML/JS/CSS không phụ thuộc Framework. Mở thẳng file `pixel-extractor-v3.html` bằng trình duyệt và sử dụng.
- Dữ liệu kết xuất cực kỳ an toàn vì mọi thuật toán xử lý luồng ảnh (`Canvas API`) đều hoạt động trên máy khách (Local Client).
