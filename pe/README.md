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

---

## 🇬🇧 English Description

An ultra-lightweight web application to convert, clean, and extract authentic 8-Bit pixel matrices from photographs, blurry images, or AI-generated artifacts (JPEG Noise/Anti-aliasing blur).
Specially optimized to generate image data arrays for precise HTML5 Canvas rendering.

![Usage Simulation](Screenshot%202026-03-08%20160708.png)

### Key Features (Version 3)

- **Real-Time Auto Sync:** Move the slider, and the preview/code updates instantly. No need to click any buttons!
- **Smart Noise Reduction:** Completely removes blurry gray/pale white halos around the subject (a very common flaw in AI-generated sprites).
- **Auto Bounding-Box:** Automatically crops the image frame, collects garbage, and eliminates useless whitespace matrices to produce the lightest and cleanest Data Array output.
- **Color Quantization:** Groups visually similar pixels (using Euclidean Distance Tolerance) into a single standard color. Extremely useful for crushing a deeply compressed, thousands-of-colors image down to its original 4-5 color palette.
- **Auto Code Gen:** Directly outputs clean JavaScript code encompassing a `Color Reference Dictionary` and an `Exact 2D Matrix (Array of Strings)`. Just copy and paste.

### Installation & Usage
- This is a pure HTML/JS/CSS tool without framework dependencies. Simply open `pixel-extractor-v3.html` in your browser to use it.
- Render data is entirely secure since all image processing algorithms (`Canvas API`) run exclusively on the local client side.
