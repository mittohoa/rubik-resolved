# RubikLab — trang giới thiệu và nơi tải app

Trang web giới thiệu **RubikLab**, ứng dụng Android dạy giải Rubik 3×3, giải khối
bằng ảnh chụp, khối ảo và bấm giờ speedcubing.

- 🌐 Trang giới thiệu: https://mittohoa.github.io/rubik-resolved/
- ⬇ Tải bản mới nhất: https://github.com/mittohoa/rubik-resolved/releases/latest
- ✉ Liên hệ: mittohoa@gmail.com

## Kho này chứa gì

| Tệp | Vai trò |
|---|---|
| `index.html` | Toàn bộ trang giới thiệu, không phụ thuộc thư viện ngoài |
| `assets/` | Biểu tượng và ảnh chụp màn hình app |
| `version.json` | Bản mới nhất — app đọc tệp này để tự báo cập nhật |
| `LICENSE` | Giấy phép MIT cho **mã nguồn trang web này** |

Mã nguồn ứng dụng RubikLab để riêng tư, không nằm trong kho này.

## Cách phát hành một bản mới

1. Tăng `version` trong `pubspec.yaml` của app, ví dụ `1.1.0+2`.
2. `flutter build apk --release`
3. Tạo release trên GitHub với thẻ `vX.Y.Z`, đính kèm tệp `RubikLab-X.Y.Z.apk`
   và ghi mã băm SHA-256 vào phần mô tả.
4. Cập nhật `version.json` ở kho này cho khớp: `versionCode`, `versionName`,
   `apkUrl`, `sizeBytes`, `sha256`, `notes`, `releasedAt`.

App sẽ tự phát hiện `versionCode` mới, hiện thông báo, tải tệp dưới nền rồi mở
trình cài đặt cho người dùng xác nhận.

## Giấy phép

Mã nguồn trang web: [MIT](LICENSE).
Ứng dụng RubikLab: miễn phí sử dụng, bản quyền © 2026 mittohoa.
