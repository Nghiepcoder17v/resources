# Fonts

## Danh sách font đang dùng trong VS Code

| Font | Dùng cho | Nguồn | Giấy phép / ghi chú |
| --- | --- | --- | --- |
| CaskaydiaCove Nerd Font Mono | Editor và terminal (font chính) | nerdfonts.com (mục Cascadia Code) | Miễn phí, mã nguồn mở |
| JetBrains Mono | Dự phòng, một số loại chữ trong CSS | jetbrains.com/lp/mono | Miễn phí, mã nguồn mở |
| Fira Code | Dự phòng, hỗ trợ ligature | github.com/tonsky/FiraCode | Miễn phí, mã nguồn mở |
| Zed Mono | Một số loại chữ trong CSS | github.com/zed-industries/zed-fonts | Miễn phí, mã nguồn mở |
| Inconsolata | Font ngoặc trong CSS dự phòng | fonts.google.com | Miễn phí, mã nguồn mở |
| Consolas | Dự phòng cuối | Có sẵn trong Windows | Của Microsoft, không phân phối lại |
| SF Mono | Ưu tiên cao trong cấu hình cũ | Apple | **Không** phân phối lại, tải từ Apple |
| Operator Mono, Dank Mono | Ưu tiên cao trong cấu hình cũ | Mua từ nhà phát hành | **Mất phí, không** đưa lên GitHub |

Cột giấy phép là ghi chú để bạn tra lại, hãy kiểm tra trang gốc của từng font trước khi chép file font vào repo.

## File danh sách

- `installed-fonts.txt`: toàn bộ font cài trên máy tại thời điểm xuất, mỗi dòng một tên.
- `vscode-fonts.txt`: chỉ các font liên quan đến VS Code, lọc từ file trên.

## Cách xuất lại danh sách (Git Bash, tại thư mục gốc của repo)

```bash
powershell -NoProfile -Command 'Add-Type -AssemblyName System.Drawing; (New-Object System.Drawing.Text.InstalledFontCollection).Families | ForEach-Object { $_.Name }' > fonts/installed-fonts.txt

grep -iE "caskaydia|jetbrains|fira code|sf mono|operator mono|dank mono|zed mono|inconsolata|consolas" fonts/installed-fonts.txt > fonts/vscode-fonts.txt
```

## Cài font trên máy mới

1. Tải font từ cột Nguồn.
2. Giải nén, chọn các file `.ttf`, chuột phải, chọn **Install for all users**.
3. Đóng hẳn và mở lại VS Code.
