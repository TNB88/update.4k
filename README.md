# Phim4K OTA Update

Ứng dụng đọc metadata cập nhật tại:

`https://raw.githubusercontent.com/TNB88/update.4k/refs/heads/main/update.json`

APK được phát hành tại GitHub Releases của repo `TNB88/FSHARE`.

## Khi có bản mới

1. Build và ký APK bằng đúng chứng thư hiện tại.
2. Tăng `version_code` trong APK và trong `update.json`.
3. Tạo Release mới ở `TNB88/FSHARE` và tải APK lên làm asset.
4. Cập nhật `download_url`, `file_size`, `checksum` và `changelog` trong `update.json`.
5. Commit `update.json` lên nhánh `main` sau khi asset Release đã sẵn sàng.

Không đổi tên các khóa JSON vì app đang đọc trực tiếp các trường `version_name`, `version_code`, `download_url`, `force_update`, `file_size`, `checksum` và `changelog`.
