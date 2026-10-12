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

## Prompt, AI Handoff và workflow v0.2.0

- **Prompt Builder:** biến brief/system/patterns thành prompt có mục tiêu, nguồn chuẩn, scope, đầu ra, tiêu chí và bằng chứng. Khi loại artifact mơ hồ, làm rõ trước khi chọn hướng triển khai. Có prompt sửa sai lệch theo output thực.
- **AI Handoff:** profile Codex, Claude (Code/chat), Devin, Kimi (CLI/chat) và generic. Giữ requirements, thay cách giao context và hướng dẫn thực hiện theo khả năng thực tế. Không tự gọi các dịch vụ này.
- **Vibe Coding Workflow:** context → UX/UI → components → screens → verify/repair → đồng bộ/bàn giao. Có thể bắt đầu ở bước phù hợp cho sửa nhỏ; lưu state/evidence/resume ở design/ai/ hoặc nơi đã có.

Ví dụ:

- “Tạo prompt cho Codex thêm Reports trong repo ReactJS/plain CSS, giữ data-table@0.1.0; kèm files cần đọc và checklist.”
- “Chuyển prompt này sang Claude Code và Kimi chat, giữ nguyên requirements; hướng dẫn tôi cung cấp context và kiểm tra.”
- “Tạo bộ prompt cho trang WEB đăng ký newsletter HTML/CSS/JS chỉ có email; chưa thực hiện code.”
- “Chạy workflow trực tiếp cho trang Settings trong repo đã có; giữ stack/local edits, ghi evidence và cập nhật screens.”
- “Tạo resume packet để đổi AI; kiểm tra sources/versions trước khi tiếp tục.”

Gói đầy đủ gồm prompt.md, execution-guide.md, acceptance-checklist.md, context-map.json và repair-prompt.md; task nhỏ có thể gộp. Chọn đúng provider/surface, cung cấp nguồn qua paths đọc được hoặc attachment/inline, làm theo guide, ghi kết quả, rồi gửi observed mismatch để repair.

Export tạo packet, không đánh dấu code đã thực hiện. Criterion required fail/not_run/thiếu evidence thì blocked; check optional chưa chạy vẫn nêu rõ. Không có bộ nhớ xuyên phiên tự động: resume cần files/revisions hiện tại. Profile có nguồn docs chưa đồng nghĩa đã test trực tiếp trên từng AI. Prompt làm rõ yêu cầu và giảm sai lệch, không bảo đảm AI luôn đúng.
