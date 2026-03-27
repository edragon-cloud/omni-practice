# Language Hub — Omni Practice Platform

Nền tảng luyện tiếng Anh tích hợp 4 ứng dụng dành cho sinh viên ĐH Đồng Nai.

## Các ứng dụng
| App | File | Mô tả |
|-----|------|--------|
| 🎙️ Fluentalk | `speak.html` | Luyện nói IELTS Speaking |
| ✍️ ArticuWrite | `write.html` | Luyện viết IELTS Writing |
| 📚 VocabMaster | `vocab.html` | Học từ vựng cho Reading |
| 🎧 ListenDictation | `listen.html` | Luyện nghe Dictation |
| 📖 Library | `library.html` | Thư viện đề IELTS Writing |

## Backend
- **GAS Backend**: Google Apps Script + Google Sheets
- **Master Sheet ID**: `1HzityqUvFG-vgdrf3uS-sOlY391ONn7tjUUuXa-Lxyk`

## Deploy
Site được host trên **GitHub Pages** tại `https://<username>.github.io/<repo>/`

### Cập nhật GAS URL
Sau khi redeploy GAS, tìm `__NEW_GAS_URL__` trong tất cả file HTML và thay bằng URL mới:
```bash
find . -name "*.html" -exec sed -i 's|__NEW_GAS_URL__|https://script.google.com/macros/s/NEW_ID/exec|g' {} +
```
