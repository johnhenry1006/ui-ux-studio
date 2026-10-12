# UI UX Studio

Plugin dành cho designer/developer: thiết kế mới, audit, triển khai frontend và quản lý pattern qua nhiều trang. Không cần Superpowers để sử dụng.

## Bắt đầu

Gọi Design Studio khi chưa rõ tác vụ, hoặc gọi workflow phù hợp: Project Brief, UX Design, UI Design, Design Audit, Frontend Implementation, Pattern Library.

- “Thiết kế app đặt lịch salon, mục tiêu giảm khách bỏ hẹn. Tạo brief, flow và bộ quy chuẩn.”
- “Audit giao diện này, ưu tiên vấn đề ảnh hưởng việc hoàn tất checkout.”
- “Thêm trang Reports trong repo hiện tại, dùng lại DataTable và cập nhật danh mục màn hình.”
- “Tạo pattern form dùng lại; ghi states, keyboard behavior và phiên bản.”

## Dữ liệu dự án

Repo: dùng `design/` hoặc nơi tương đương đã có. ChatGPT: cung cấp bộ file dự án hoặc cho phép dùng nơi lưu file mà host hỗ trợ. Khi tiếp tục phiên mới, đưa lại brief, design system, screen inventory, decisions và pattern lock; plugin phải đọc lại trước khi tiếp tục theo quy chuẩn cũ.

Thư viện cá nhân: chọn folder riêng; gợi ý `UI-UX-Studio/preferences.md` và `UI-UX-Studio/patterns/` ngoài từng repo. Catalog đóng gói chỉ là seed; không sửa package để lưu dự án. Project references lưu nơi truy cập được, không có đồng bộ nền hay bộ nhớ xuyên phiên tự động.

## Công nghệ

Dự án mới: ReactJS + JavaScript + CSS thuần hoặc HTML/CSS/JavaScript. Không tự thêm Next.js, TypeScript, Tailwind. Repo có sẵn theo stack/components/styling hiện tại; không tự migration. Web apps nằm trong phạm vi code; app native được tư vấn UI/UX.

## Giới hạn

Plugin là hướng dẫn + templates, không có server/Figma integration. Host quyết định có đọc repo, sửa code, lưu file, xem ảnh hay mở browser hay không. Ảnh tĩnh không chứng minh hành vi tương tác. Plugin phải báo checks đã chạy và phần chưa kiểm chứng; không tuyên bố đã cài/hoạt động chỉ vì package được tạo.
