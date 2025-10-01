📝 HƯỚNG DẪN GIT ADD -P (PATCH MODE)

Khi chạy `git add -p <file>`, Git sẽ hiển thị từng hunk (khối thay đổi) và hỏi:
"Stage this hunk [y,n,q,a,d,s,e,p,?]?"

CÁC LỰA CHỌN CHÍNH:
✅ y = yes: Stage hunk này
❌ n = no: Bỏ qua hunk này  
🚪 q = quit: Thoát khỏi patch mode
📦 a = all: Stage hunk này và tất cả hunks còn lại
🗑️ d = don't: Bỏ qua hunk này và tất cả hunks còn lại

CÁC LỰA CHỌN NÂNG CAO:
✂️ s = split: Chia hunk thành các phần nhỏ hơn (nếu có thể)
✏️ e = edit: Chỉnh sửa hunk bằng editor
👀 p = print: Hiển thị lại hunk hiện tại
❓ ? = help: Hiển thị trợ giúp

LỢI ÍCH CỦA GIT ADD -P:
- Cho phép staging từng phần thay đổi
- Tạo commits có ý nghĩa rõ ràng
- Tránh commit nhầm code không liên quan
- Kiểm soát chính xác nội dung commit