📋 SO SÁNH: GIT RESTORE vs GIT CHECKOUT --

🆕 GIT RESTORE (từ Git 2.23+) - KHUYẾN NGHỊ SỬ DỤNG:
┌─────────────────────────────────────────────────┐
│ CHUYÊN DỤNG CHO VIỆC RESTORE FILE              │
│                                                 │
│ git restore <file>           # Restore từ index│
│ git restore --staged <file>  # Unstage file    │
│ git restore --source=HEAD~1 <file> # Từ commit│
│                                                 │
│ ✅ Cú pháp rõ ràng, dễ hiểu                    │
│ ✅ Chỉ làm một việc: restore file              │
│ ✅ An toàn hơn, ít nhầm lẫn                    │
└─────────────────────────────────────────────────┘

🔄 GIT CHECKOUT -- (cũ) - ĐANG BỊ DEPRECATED:
┌─────────────────────────────────────────────────┐
│ ĐA CHỨC NĂNG - DỄ NHẦM LẪN                     │
│                                                 │
│ git checkout -- <file>       # Restore file    │
│ git checkout <branch>        # Chuyển nhánh    │
│ git checkout -b <branch>     # Tạo nhánh mới   │
│                                                 │
│ ❌ Cú pháp khó hiểu với "--"                   │
│ ❌ Dễ nhầm với chuyển nhánh                    │
│ ❌ Một lệnh nhiều chức năng                    │
└─────────────────────────────────────────────────┘

DEMO THỰC TẾ:
Thay đổi file này và thử:
- git restore demo-restore.md
- git checkout -- demo-restore.md