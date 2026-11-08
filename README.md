# resources

Kho tài nguyên cá nhân: danh sách font, hình nền và các file dùng chung giữa các máy.

## Cấu trúc

| Thư mục / File | Nội dung |
| --- | --- |
| `fonts/` | Danh sách font đã cài, nguồn tải và giấy phép (không chứa file font có bản quyền) |
| `wallpapers/` | Hình nền, gồm ảnh nền VS Code |
| `.gitignore` | Loại các file không nên đưa lên GitHub |

## Quy tắc của repo này

- Repo ở chế độ **public**, nên chỉ để những thứ có thể công khai.
- Font: lưu **tên và nguồn tải**. Chỉ chép file `.ttf` khi giấy phép cho phép phân phối lại.
- File cá nhân hoặc riêng tư (giấy tờ, ảnh cá nhân, khóa, mật khẩu) **không** để ở đây.
- Mỗi file ảnh nên dưới 5 MB. GitHub từ chối file trên 100 MB.

## Dùng ảnh nền làm nền VS Code

Link trực tiếp tới ảnh có dạng:

```
https://raw.githubusercontent.com/TEN-BAN/resources/main/wallpapers/TEN-FILE.png
```

Dán link này vào mục `images` của `background.fullscreen` trong `settings.json` (repo `backup-vscode`).
